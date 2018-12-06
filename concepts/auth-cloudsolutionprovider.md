---
title: Aufrufen von Microsoft Graph aus einer Anwendung eines Cloud-Lösungsanbieters
description: In diesem Thema wird beschrieben, wie Sie Anwendungszugriff auf partnerverwaltete Kundendaten über Microsoft Graph aktivieren, entweder mit dem Fluss zur Erteilung von Autorisierungscodes oder dem Fluss zur Gewährung von Clientanmeldeinformationen für Dienst-zu-Dienst-Aufrufe.
ms.openlocfilehash: a14c610090a1232c72ec2fde4469dd1cd1d6f694
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092246"
---
# <a name="call-microsoft-graph-from-a-cloud-solution-provider-application"></a>Aufrufen von Microsoft Graph aus einer Anwendung eines Cloud-Lösungsanbieters

> **Hinweis:** Dieses Thema gilt **nur** für Microsoft CSP-Anwendungsentwickler (Cloud-Lösungsanbieter). Das Programm [Microsoft Cloud-Lösungsanbieter (CSP)](https://partner.microsoft.com/de-DE/cloud-solution-provider) ermöglicht es Microsoft-Partnern, Microsoft Onlinedienste an Kunden zu verkaufen und zu verwalten.

In diesem Thema wird beschrieben, wie Sie Anwendungszugriff auf partnerverwaltete Kundendaten über Microsoft Graph aktivieren, entweder mit dem [Fluss zur Erteilung von Autorisierungscodes](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-protocols-oauth-code) oder dem [Fluss zur Gewährung von Clientanmeldeinformationen für Dienst-zu-Dienst-Aufrufe](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service).

**Wichtig:** Das Aufrufen von Microsoft Graph aus einer CSP-Anwendung wird nur für Verzeichnisressourcen (z. B. **user**, **group**,**device**, **organization**) und [Intune](/graph/api/resources/intune-graph-overview?view=graph-rest-beta)-Ressourcen unterstützt.

## <a name="what-is-a-partner-managed-application"></a>Was ist eine partnerverwaltete Anwendung?

Das CSP-Programm ermöglicht es Microsoft-Partnern, Microsoft-Onlinedienste (z. B. Office 365, Microsoft Azure und CRM Online) an Kunden zu verkaufen und zu verwalten. Die Verwaltung von Kundendiensten erfolgt über delegierte Administratorberechtigungen, wodurch festgelegte Partnerbenutzer (als Agenten bezeichnet) auf die Umgebungen ihrer Kunden zugreifen und diese konfigurieren können.

Darüber hinaus können Sie als Partnerentwickler eine **partnerverwaltete App** zum Verwalten der Microsoft-Dienste Ihrer Kunden erstellen. Partnerverwaltete Apps werden oft als *vorab genehmigte* Apps bezeichnet, da alle Ihre Kunden automatisch vorab für Ihre partnerverwalteten Apps genehmigt werden. Dies bedeutet Folgendes: Wenn ein Benutzer aus einem Ihrer Kundenmandanten eine Ihrer partnerverwalteten Apps verwendet, kann der Benutzer die App nutzen, ohne dass er zur Zustimmung aufgefordert wird. Partnerverwaltete Apps erben außerdem delegierte Administratorberechtigungen, sodass Ihre Partneragenten über Ihre partnerverwaltete Anwendung ebenfalls privilegierten Zugriff auf Ihre Kunden erhalten.

## <a name="how-to-set-up-a-partner-managed-application"></a>Einrichten einer partnerverwalteten Anwendung

Eine Anwendung wird als *partnerverwaltet* betrachtet, wenn ihr erhöhte Rechte zum Zugreifen auf die Daten Ihrer Kunden gewährt werden.

> **Hinweis:** Partnerverwaltete Apps können *nur* auf Partnermandanten konfiguriert werden, und zum Verwalten von Ressourcen des Kundenmandanten **müssen** partnerverwaltete Apps als **mehrinstanzenfähige Anwendungen** konfiguriert werden.

### <a name="register-and-configure-a-multi-tenant-app"></a>Registrieren und Konfigurieren einer mehrinstanzenfähigen App

Die ersten hier erforderlichen Schritte entsprechen weitgehend den Schritten zum Registrieren und Konfigurieren einer mehrinstanzenfähigen Anwendung:

1. [Registrieren Sie die Anwendung](https://docs.microsoft.com/de-DE/azure/active-directory/active-directory-app-registration) in Ihrem Partnermandanten über das [Azure-Portal](https://portal.azure.com). Um als partnerverwaltete App ausgeführt werden zu können, muss eine Anwendung als [mehrinstanzenfähige App](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#update-registration-to-be-multi-tenant) konfiguriert werden. Falls Ihre App in mehreren geografische Regionen bereitgestellt und verkauft wird, müssen Sie Ihre App außerdem in jeder dieser Regionen registrieren, wie <a href="#region">hier</a> beschrieben.
2. Konfigurieren Sie Ihre mehrinstanzenfähige App über das Azure-Portal mit den *erforderlichen Berechtigungen*; verwenden Sie einen Ansatz geringster Rechte.

### <a name="pre-consent-your-app-for-all-your-customers"></a>Vorabgenehmigen Ihrer App für alle Ihre Kunden

Zum Schluss gewähren Sie Ihrer partnerverwalteten App diese konfigurierten Berechtigungen für alle Ihre Kunden. Hierzu können Sie den **servicePrincipal**, der die App darstellt, mithilfe von Azure AD PowerShell V2 zur Gruppe *Adminagents* in Ihrem Partnermandanten hinzufügen. Sie können Azure AD PowerShell V2 [hier](https://www.powershellgallery.com/packages/AzureAD) herunterladen und installieren.  Führen Sie die folgenden Schritte aus, um die Gruppe *Adminagents* und den **servicePrincipal** zu suchen und ihn zur Gruppe hinzuzufügen.

1. Öffnen Sie eine PowerShell-Sitzung und stellen Sie eine Verbindung mit Ihrem Partnermandanten her, indem Sie Ihre Administrator-Anmeldeinformationen in das Anmeldefenster eingeben.

    ```PowerShell
    Connect-AzureAd
    ```

2. Suchen Sie die Gruppe, die die *Adminagents* darstellt.

    ```PowerShell
    $group = Get-AzureADGroup -Filter "displayName eq 'Adminagents'"
    ```

3. Suchen Sie den Dienstprinzipal, der die gleiche *appId* hat wie Ihre App.

    ```PowerShell
    $sp = Get-AzureADServicePrincipal -Filter "appId eq '{yourAppsAppId}'"
    ```

4. Fügen Sie zum Schluss den Dienstprinzipal zur Gruppe *Adminagents* hinzu.

    ```PowerShell
    Add-AzureADGroupMember -ObjectId $group.ObjectId -RefObjectId $sp.ObjectId
    ```

## <a name="token-acquisition-flows"></a>Tokenerwerbsflüsse

Die Tokenerwerbsflüsse für partnerverwaltete Apps – [Fluss zur Erteilung von Autorisierungscodes](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-protocols-oauth-code) und [Fluss zur Gewährung von Clientanmeldeinformationen für Dienst-zu-Dienst-Aufrufe](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service) – sind dieselben wie für normale mehrinstanzenfähige Apps.

Abgesehen vom vorab genehmigten Zugriff auf alle Ihre Kundenmandanten haben partnerverwaltete Apps eine zusätzliche Fähigkeit. Sie ermöglicht es Ihren Agenten, mit Ihrer App auf Mandantendaten Ihres Kunden zuzugreifen (mit delegierten Administratorrechten). Im Prinzip funktioniert es wie folgt:

1. Der Agent meldet sich mit seinen Benutzeranmeldeinformationen, die von Ihrem Partnermandanten ausgestellt wurden, bei Ihrer App an.
2. Die App fordert ein Zugriffstoken für den gewünschten partnerverwalteten Kundenmandanten an.
3. Die App ruft unter Verwendung des Zugriffstokens Microsoft Graph auf.

Dies ist ein standardmäßiger [Fluss zur Erteilung von Autorisierungscodes](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-protocols-oauth-code), mit der Ausnahme, dass Ihre Agenten sich mit ihren Partnerkonten anmelden müssen. Um anzuzeigen, wie dies aussieht, stellen Sie sich vor, Ihr Partnermandant ist *partner.com* (dies ist die Startmandant für Ihre Agenten) und einer Ihrer Kunden ist *customer.com*:

1. [Autorisierungscode erwerben:](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-protocols-oauth-code#request-an-authorization-code) Die App sendet eine Anforderung an den Endpunkt ```/authorize``` und muss einen **Kundenmandanten**, in unserem Beispiel ```customer.com```, als Mandantenziel verwenden. Ihre Agenten melden sich weiterhin mit ihrem ```username@partner.com```-Konto an.

    ```http
    GET https://login.microsoftonline.com/customer.com/oauth2/authorize
    ```

2. [Zugriffstoken mithilfe des Autorisierungscodes erwerben:](https://docs.microsoft.com/de-DE/azure/active-directory/develop/active-directory-protocols-oauth-code#use-the-authorization-code-to-request-an-access-token) Ihre App muss einen **Kundennandanten** als Zielmandanten verwenden, in unserem Beispiel ```customer.com```, wenn sie die Anforderung an den Endpunkt ```token``` sendet:

    ```http
    POST https://login.microsoftonline.com/customer.com/oauth2/token
    ```

3. Nachdem Sie jetzt über ein Zugriffstoken verfügen, rufen Sie Microsoft Graph auf, und fügen Sie das Zugriffstoken in den HTTP-Autorisierungsheader ein:

    ```http
    GET https://graph.microsoft.com/beta/users
    Authorization: Bearer <token>
    ```

## <a name="register-your-app-in-the-regions-you-support"></a>Registrieren Ihrer App in den von Ihnen unterstützten Regionen
<a name="region"></a>

Die Kundenbeteiligung am CSP-Programm ist derzeit auf eine einzige Region beschränkt. Für partnerverwaltete Anwendungen gilt dieselbe Einschränkung. Dies bedeutet, dass Sie einen separaten Mandanten für jede Regionen benötigen, in der Sie verkaufen. Wenn Ihre partnerverwaltete App beispielsweise in einem Mandanten in den USA registriert ist, Ihr Kunde aber in der EU sitzt, funktioniert die partnerverwaltete App nicht.  Jeder Ihrer regionalen Partnermandanten muss einen eigenen Satz partnerverwalteter Apps pflegen, um Kunden innerhalb der gleichen Region zu verwalten. Dies erfordert möglicherweise zusätzliche Logik in Ihrer App (vor der Anmeldung) zum Abrufen des Anmeldebenutzernamen Ihres Kunden, um zu entscheiden, welche regionsspezifische partnerverwaltete App-Identität für den Benutzer verwendet werden soll.

## <a name="calling-microsoft-graph-immediately-after-customer-creation"></a>Aufrufen von Microsoft Graph sofort nach dem Erstellen des Kunden

Wenn Sie einen neuen Kunden mit der [Partner Center-API](https://partnercenter.microsoft.com/de-DE/partner/developer) erstellen, wird ein neuer Kundenmandant erstellt. Darüber hinaus wird eine Partnerbeziehung erstellt, wodurch Sie zum gespeicherten Partner dieses neuen Kundenmandanten werden. Es kann bis zu drei Minuten dauern, bis diese Partnerbeziehung an den neuen Kundenmandanten verteilt wird. Wenn Ihre App Microsoft Graph direkt nach der Erstellung aufruft, erhält die App wahrscheinlich die Fehlermeldung, dass der Zugriff verweigert wurde. Eine ähnliche Verzögerung kann eintreten, wenn ein bestehender Kunde Ihre Einladung akzeptiert. Dies liegt daran, dass die Vorabzustimmung davon abhängt, dass die Partnerbeziehung im Kundenmandanten vorhanden ist.

Um dieses Problem zu vermeiden, wird empfohlen, dass die Partner-App nach der Kundenerstellung **drei Minuten** warten sollte, bevor sie Azure AD zum Erwerb eines Tokens (für den Aufruf von Microsoft Graph) aufruft. Hiermit sollten die meisten Fälle abgedeckt sein. Wenn jedoch nach Verstreichen der Wartezeit von drei Minuten weiterhin ein Autorisierungsfehler ausgegeben wird, warten Sie weitere 60 Sekunden, und versuchen Sie es erneut.

> **Hinweis:** Bei der Wiederholung müssen Sie ein neues Zugriffstoken von Azure AD erwerben, bevor Sie Microsoft Graph aufrufen.  Der Aufruf von Microsoft Graph mit dem bereits vorhandenen Zugriffstoken funktioniert nicht, da das Zugriffstoken nur eine Stunde lang gültig ist und die vorab genehmigten Berechtigungsansprüche nicht enthält.
