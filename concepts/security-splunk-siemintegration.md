---
title: Integrieren von Microsoft Graph Sicherheit API Benachrichtigungen in Ihrer SIEM mit Azure Systemmonitor
description: Die Microsoft Graph-Sicherheitsanbieter können über einen einzelnen REST-Endpunkt verwaltet werden. Diesen Endpunkt kann mit Azure Monitor konfiguriert werden die Konnektoren für mehrere SIEM Produkte unterstützt. Die Anweisungen in Schritt 1 und 2 dieses Artikels finden Sie alle Azure Monitor Connectors, die Auslastung über Ereignis Hubs unterstützen. Dieser Artikel beschreibt die End-to-End-Integration der Splunk SIEM Verbindung.
ms.openlocfilehash: bdd1d1e192a4945c67727d20e594006a387fb156
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092273"
---
# <a name="integrate-microsoft-graph-security-api-alerts-with-your-siem-using-azure-monitor"></a>Integrieren von Microsoft Graph Sicherheit API Benachrichtigungen in Ihrer SIEM mit Azure Systemmonitor

Die Microsoft Graph-Sicherheitsanbieter können über einen einzelnen REST-Endpunkt verwaltet werden. Diesen Endpunkt kann mit [Azure Monitor](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/) konfiguriert werden die Konnektoren für mehrere SIEM Produkte unterstützt. Die Anweisungen in Schritt 1 und 2 dieses Artikels finden Sie alle Azure Monitor Connectors, die Auslastung über Ereignis Hubs unterstützen. Dieser Artikel beschreibt die End-to-End-Integration der [Splunk](https://splunkbase.splunk.com/) SIEM Verbindung.

Der Integrationsvorgang umfasst die folgenden Schritte:

1. [Einrichten von Azure-Ereignis Hub Sicherheitshinweise für Ihre Mandanten empfangen](#step-1-set-up-an-event-hubs-namespace-in-azure-to-receive-security-alerts-for-your-tenant)
2. [Konfigurieren von Azure Monitor zum Senden von Sicherheitswarnungen vom Mandanten an den Event Hub](#step-2-configure-azure-monitor-to-send-security-alerts-from-your-tenant-to-the-event-hub)
3. [Herunterladen und Installieren des Azure Monitor-Add-Ons für Splunk, das es Splunk ermöglicht, Sicherheitswarnungen zu verbrauchen](#step-3-download-and-install-the-azure-monitor-add-on-for-splunk-which-will-allow-splunk-to-consume-security-alerts)
4. [Registrieren einer Anwendung bei dem Azure Active Directory des Mandanten, das Splunk verwendet, um Lesevorgänge vom Event Hub durchzuführen](#step-4-register-an-application-with-your-tenant-azure-active-directory-which-splunk-will-use-to-read-from-the-event-hub )
5. [Erstellen eines Azure Key Vault zum Speichern der Zugriffsschlüssel für den Event Hub](#step-5-create-an-azure-key-vault-to-store-the-access-key-for-the-event-hub)
6. [Konfigurieren der Splunk-Dateneingaben zum Verbrauchen von Sicherheitswarnungen, die im Event Hub gespeichert sind](#step-6-configure-the-splunk-data-inputs-to-consume-security-alerts-stored-in-the-event-hub)

Nachdem Sie diese Schritte durchgeführt haben, verbraucht Ihre Splunk Enterprise die Sicherheitswarnungen aller Sicherheitsprodukte, die in Microsoft Graph integriert sind und für die Ihr Mandant lizenziert ist. Alle neuen Sicherheitsprodukte, die Sie lizenzieren, senden ebenfalls Warnungen über diese Verbindung, und zwar in demselben Schema und ohne weiteren Integrationsaufwand.

## <a name="step-1-set-up-an-event-hubs-namespace-in-azure-to-receive-security-alerts-for-your-tenant"></a>Schritt 1: Einrichten eines Event Hub-Namespace in Azure zum Empfangen von Sicherheitswarnungen für Ihren Mandanten

Um zu beginnen, müssen Sie einen [Microsoft Azure Ereignis Hubs](https://docs.microsoft.com/en-us/azure/event-hubs/) Namespace und Ereignis Hub Anlegens. Dieser Namespace und Event Hub ist das Ziel für alle Sicherheitswarnungen in Ihrer Organisation. Ein Event Hub-Namespace ist eine logische Gruppierung von Event Hubs, die dieselbe Zugriffsrichtlinie verwenden. Beachten Sie einige Details zum Event Hub-Namespace und den Event Hubs, die Sie erstellen:

- Wir empfehlen die Verwendung eines standardmäßigen Event Hub-Namespace, insbesondere dann, wenn Sie andere Azure-Überwachungsdaten über dieselben Event Hubs senden.
- In der Regel ist nur eine Durchsatzeinheit erforderlich. Wenn sich die Nutzung erhöht und sie nach oben skalieren müssen, können Sie die Anzahl der Durchsatzeinheiten für den Namespace später immer noch manuell erhöhen oder die automatische Erhöhung aktivieren.
- Die Anzahl der Durchsatzeinheiten ermöglicht Ihnen, den Durchsatzmaßstab für die Event Hubs zu erhöhen. Die Anzahl der Partitionen ermöglicht Ihnen, den Verbrauch für viele Kunden zu parallelisieren. Eine einzelne Partition kann bis zu 20 MBit/s erzielen bzw. ungefähr 20.000 Nachrichten pro Sekunde. Abhängig von dem Tool, das die Daten verbraucht, wird der Verbrauch durch mehrere Partitionen unterstützt oder auch nicht. Wenn Sie nicht sicher sind, wie viele Partitionen Sie festlegen sollen, empfehlen wir, mit vier Partitionen zu beginnen.
- Wir empfehlen, dass Sie die Nachrichtenaufbewahrung für Ihren Event Hub auf 7 Tage festlegen. Sollte das verbrauchende Tool länger als einen Tag ausfällt, wird hierdurch sichergestellt, dass das Tool dort fortfahren kann, wo es aufgehört hat (für Ereignissen, die bis zu sieben Tage alt sind).
- Wir empfehlen die Verwendung der standardmäßigen Consumergruppe für Ihren Event Hub. Sie müssen keine anderen Consumergruppen erstellen und keine separate Consumergruppe verwenden, es sei denn, Sie haben zwei verschiedene Tools, die dieselben Daten von demselben Event Hub verbrauchen.
- In der Regel müssen Port 5671 und 5672 auf dem Computer geöffnet sein, der die Daten vom Event Hub verbraucht.

Weitere Informationen finden sie auch unter [Häufig gestellte Fragen zu Azure Event Hubs](https://docs.microsoft.com/en-us/azure/event-hubs/event-hubs-faq).

1. Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an, und wählen Sie **Ressource erstellen** oben links auf dem Bildschirm.

    ![Bild zu „Ressource erstellen“](images/create-resource.png)

2. Wählen Sie **Internet of Things** und dann **Event Hubs**.

    ![Abbildung zu Event Hubs](images/event-hubs.png)

3. Geben Sie unter **Namespace erstellen** einen Namen für den Namespace ein. Nachdem Sie sichergestellt haben, dass der Name des Namespace verfügbar ist, wählen Sie den Tarif aus (Basic oder Standard). Wählen Sie außerdem ein Azure-Abonnement, eine Ressourcengruppe und einen Speicherort, an dem die Ressource erstellt werden soll. Wählen Sie **Erstellen**, um den Namespace zu erstellen. Sie müssen möglicherweise einige Minuten warten, bis das System die Ressourcen vollständig bereitgestellt hat.

    ![Abbildung zu „Namespace erstellen“](images/create-namespace.png)

## <a name="step-2-configure-azure-monitor-to-send-security-alerts-from-your-tenant-to-the-event-hub"></a>Schritt 2: Konfigurieren von Azure Monitor zum Senden von Sicherheitswarnungen vom Mandanten an den Event Hub

Das Aktivieren des Streamings von Sicherheitswarnungen Ihrer Organisation über Azure Monitor erfolgt einmal für den gesamten Azure Active Directory (Azure AD)-Mandanten. Alle Microsoft Graph Sicherheit API lizenziert, und senden Sicherheitshinweise an Azure Monitor, streaming von Daten zum Verarbeiten von Applikationen aktivierte Produkten beginnt. Eine beliebige zusätzlichen Microsoft Graph Sicherheit API-fähigen Produkten lizenziert und von Ihrer Organisation bereitgestellt werden automatisch Sicherheitshinweise über derselben Azure Monitor Konfiguration gestreamt. Es ist kein weiterer Integrationsaufwand durch Ihre Organisation erforderlich.

Sicherheitswarnungen sind Daten mit der höchsten Berechtigungsstufe, die in der Regel nur für Sicherheitsexperten und globale Administratoren in einer Organisation angezeigt werden. Aus diesem Grund benötigen Sie ein globales Administratorkonto für Azure AD, um die erforderlichen Schritte zum Konfigurieren der Integration von Sicherheitswarnungen mit SIEM-Systemen zu konfigurieren. Sie benötigen dieses Konto nur einmal während des Setups, um anzufordern, dass die Sicherheitswarnungen Ihrer Organisation an Azure Monitor gesendet werden.

> **Hinweis:** Das Azure Monitor Diagnostic Einstellungen Blade unterstützt derzeit keine Konfiguration auf Mandantenebene Ressourcen. Microsoft Graph Sicherheit API bei Benachrichtigungen handelt es sich um eine Ressource auf Mandantenebene, die erforderlich sind, mit der Azure-Ressourcen-Manager-API Azure Monitor zur Unterstützung der Auslastung Sicherheitshinweise für Ihre Organisation konfigurieren.

1. Registrieren Sie in Ihrem Azure-Abonnement „microsoft.insights“ (Azure Monitor) als Ressourcenanbieter.  
 > **Hinweis:** Registrieren Sie "Microsoft.SecurityGraph" (Microsoft Graph Sicherheit API) nicht als Ressourcenanbieter für die in der Azure-Abonnement, wie "Microsoft.SecurityGraph" eine Ressource auf Mandantenebene ist, wie oben beschrieben. Die Konfiguration auf Mandantenebene werden ist Teil von Nr. 6 weiter unten.

2. Um Azure Monitor mithilfe der Azure Resource Manager-API zu konfigurieren, besorgen Sie sich das [ARMClient](https://github.com/projectkudu/ARMClient)-Tool. Dieses Tool wird verwendet, um REST-API-Aufrufe über die Befehlszeile an das Azure-Portal zu senden.

3. Erstellen Sie eine JSON-Datei mit Diagnose-Einstellungen wie die folgende:

<!-- {
  "blockType": "ignored"
} -->

    ``` json
    {
      "location": "",
      "properties": {
        "name": "securityApiAlerts",
        "serviceBusRuleId": "/subscriptions/SUBSCRIPTION_ID/resourceGroups/RESOURCE_GROUP/providers/Microsoft.EventHub/namespaces/EVENT_HUB_NAMESPACE/authorizationrules/RootManageSharedAccessKey",
        "logs": [
          {
            "category": "Alert",
            "enabled": true,
            "retentionPolicy": {
              "enabled": true,
              "days": 7
            }
          }
        ]
      }
    }
    ```

  Ersetzen Sie die Werte in der JSON-Datei wie folgt:

  * **SUBSCRIPTION_ID** ist die Abonnement-ID des Azure-Abonnements, das die Ressourcengruppe hostet und der Event Hub-Namespace, an den Sie Sicherheitswarnungen von Ihrer Organisation senden.
  * **RESOURCE_GROUP** ist die Ressourcengruppe mit dem Ereignis Hub-Namespace, an den Sie Sicherheitswarnungen von Ihrer Organisation senden.
  * **EVENT_HUB_NAMESPACE** ist der Event Hub-Namespace, an den Sie Sicherheitswarnungen von Ihrer Organisation senden.
  * **"Tage":** ist die Anzahl der Tage, die Nachrichten in Ihrem Haupt-Ereignis erhalten bleiben soll.
  
&nbsp;
4. Speichern Sie die Datei als JSON in dem Verzeichnis, in dem Sie „ARMClient.exe“ aufrufen. Nennen Sie die Datei zum Beispiel **AzMonConfig.json.**

5. Führen Sie den folgenden Befehl aus, um sich beim ARMClient-Tool anzumelden. Sie müssen Anmeldedaten eines globalen Administratorkontos verwenden.

    ``` shell
    ARMClient.exe login
    ```

6. Führen Sie den folgenden Befehl aus, um Azure Monitor so zu Konfigurieren, dass Sicherheitswarnungen an den Event Hub-Namespace gesendet werden. Dadurch wird automatisch einen Event Hub innerhalb des Namespace bereitgestellt und der Fluss von Sicherheitswarnungen an den Event Hub begonnen. Stellen Sie sicher, dass der Name der Einstellung (in diesem Beispiel **securityApiAlerts**) dem Einstellungsnamen entspricht, den Sie in der JSON-Datei für das Feld **name** angegeben haben.

    ``` shell
    ARMClient.exe put https://management.azure.com/providers/Microsoft.SecurityGraph/diagnosticSettings/securityApiAlerts?api-version=2017-04-01-preview  @".\AzMonConfig.json"
    ```

7. Um sicherzustellen, dass die Einstellungen richtig angewendet wurden, führen Sie diesen Befehl aus, und stellen Sie sicher, dass die Ausgabe den JSON-Dateieinstellungen entspricht.

    ``` shell
    ARMClient.exe get https://management.azure.com/providers/Microsoft.SecurityGraph/diagnosticSettings/securityApiAlerts?api-version=2017-04-01-preview
    ```

8. Beenden Sie das ARMClient-Tool. Sie haben jetzt die Konfiguration von Azure Monitor zum Senden von Sicherheitswarnungen von Mandanten an den Event Hub abgeschlossen.

## <a name="step-3-download-and-install-the-azure-monitor-add-on-for-splunk-which-will-allow-splunk-to-consume-security-alerts"></a>Schritt 3: Herunterladen und Installieren des Azure Monitor-Add-Ons für Splunk, das es Splunk ermöglicht, Sicherheitswarnungen zu verbrauchen

1. Diese Integration unterstützt nur [Splunk Enterprise](https://splunkbase.splunk.com/) -Bereitstellungen.
2. Laden Sie das [Azure Monitor-Add-On für Splunk](https://github.com/Microsoft/AzureMonitorAddonForSplunk) herunter, und installieren Sie es. Ausführliche Installationsanweisungen finden Sie unter [Installation](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Installation). **Nur Azure Monitor Add-on für Splunk Version 1.2.9 oder höher unterstützt.**
3. Führen Sie nach der erfolgreichen Installation von Add-Ons, im [Azure Monitor Add-on Konfiguration Wiki](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Configuration-of-Splunk ) -Splunk konfigurieren erläuterten Konfigurationsschritte aus.
4. Wie in den Installationsanweisungen zum Add-On angegeben, funktioniert das Add-On, sobald Sie einen Deaktivieren-Aktivieren-Zyklus auf der Seite „Manage Apps“ in Splunk Web ausgeführt  haben. Sie können Splunk auch neu starten.

## <a name="step-4-register-an-application-with-your-tenant-azure-active-directory-which-splunk-will-use-to-read-from-the-event-hub"></a>Schritt 4: Registrieren einer Anwendung bei dem Azure Active Directory des Mandanten, das Splunk verwendet, um Lesevorgänge vom Event Hub durchzuführen

Splunk benötigt eine Anwendung Registrierung in Ihrer Organisation Azure Active Directory die erforderlichen Berechtigungen und app-Anmeldeinformationen an den Monitor Azure-Ereignis Hub authentifizieren erteilt werden.

1. Gehen Sie im Azure-Portal zu **App-Registrierungen**, und wählen Sie **Registrierung einer neuen Anwendung** aus.

    ![Bild „App-Registrierung“](images/app-registration.png)

2. Wählen Sie einen Namen für die Anwendung aus, wählen Sie **Web-App/API** als Typ, und **`https://localhost`** als URL für die Anmeldung. Wählen Sie dann **Erstellen** aus.

    ![Web-API-Konfiguration](images/app-web-config.png)

3. Nachdem die Anwendung erstellt wurde, kopieren Sie die **Anwendungs-ID**, und speichern Sie sie zur späteren Verwendung beim Konfigurieren der Splunk Dateneingaben. Wechseln Sie dann zu den Anwendungseinstellungen, und wählen Sie **Schlüssel**.

    ![Web-App-ID](images/app-id.png)

    Hierdurch können Sie einen neuen Schlüssel generieren, der als „geheimer Anwendungsschlüssel“ bezeichnet wird. Nachdem er generiert wurde, kopieren Sie den **geheimen Anwendungsschlüssel**, und speichern Sie ihn zur späteren Verwendung beim Konfigurieren der Splunk-Dateneingaben.

4. Erteilen Sie der Anwendung die Rolle **Leser** im Azure-Abonnement mit dem Event Hub, der die Sicherheitswarnungen Ihrer Organisation enthält.

    ![Azure-Abo hinzufügen](images/add-azure-sub.png)

    Wählen Sie Ihr Abonnement, wählen Sie **Zugriffssteuerung (IAM)**. Wählen Sie **Hinzufügen**, um Berechtigungen hinzuzufügen. Wählen Sie Ihre Anwendung aus, und wählen Sie als **Rolle** für die Anwendung **Leser**.

    ![Leser-Berechtigung hinzufügen](images/add-reader-perms.png)

    Wählen Sie **Speichern**, um die gewährten Berechtigungen der Anwendung zum Abonnement hinzuzufügen.

## <a name="step-5-create-an-azure-key-vault-to-store-the-access-key-for-the-event-hub"></a>Schritt 5: Erstellen eines Azure Key Vault zum Speichern der Zugriffsschlüssel für den Event Hub

Azure Key Vaults dienen zum Speichern von Geheimnissen wie Identitäten, Kennwörtern und Zertifikaten für die Verwendung zur Laufzeit durch Anwendungen. In diesem Schritt erstellen Sie einen Azure Key Vault zum Speichern der Geheimnisse, die Splunk benötigt, um eine Verbindung mit Azure-Event-Hubs herzustellen und die darin enthaltenen Sicherheitswarnungen zu lesen.

1. Wechseln Sie im Azure-Portal zu **Key Vaults**, und wählen Sie **Hinzufügen** aus.

    ![Key Vaults hinzufügen](images/add-key-vaults.png)

2. Wählen Sie beim Erstellen des neuen Key Vaults **Zugriffsrichtlinien**, um eine neue Zugriffsrichtlinie für die Anwendung hinzuzufügen, die Sie gerade in Schritt 4 registriert haben. Gewähren Sie der Anwendung die Berechtigung **Get**. Dadurch kann Splunk, das als registrierte Anwendung fungiert, auf die in diesem Azure Key Vault gespeicherten Schlüssel (Geheimnisse) zugreifen.

    ![Zugriffsrichtlinien hinzufügen](images/add-access-policies.png)

    Wählen Sie **Erstellen**, um die Erstellung Ihres neuen Azure Key Vault abzuschließen.

3. Generieren Sie einen neuen geheimen Schlüssel im Key Vault, um den Zugriffsschlüssel für den Event Hub-Namespace zu speichern. Rufen Sie zuerst den Zugriffsschlüssel für den Event Hub-Namespace ab, indem Sie den Event Hub-Namespace öffnen und die Option **Freigegebene Zugriffsrichtlinien** auswählen. Wählen Sie die **RootManageSharedAccessKey**-Richtlinie aus der Liste, und kopieren Sie den **Primärschlüssel** aus der Liste.

    ![Freigegebene Zugriffsrichtlinien abrufen](images/get-shared-policies.png)

4. Öffnen Sie den Key Vault, und wählen Sie **Geheimnisse**. Wählen Sie **Generieren/Importieren**, um dem Key Vault ein neues Geheimnis hinzuzufügen. Fügen Sie den **Primärschlüssel** aus dem Event Hub-Namespace **RootManageSharedAccessKey** ein.

    ![Neuen geheimen Schlüssel generieren](images/generate-new-secret.png)

5. Nachdem es erstellt wurde, wählen Sie das Geheimnis aus, und kopieren Sie die **Geheimnisversion** des Geheimnisses. Dies wird weiter unten in Schritt 6 verwendet, um Splunk-Dateneingaben zu konfigurieren.

    ![Version des geheimen Schlüssels](images/secret-version.png)

## <a name="step-6-configure-the-splunk-data-inputs-to-consume-security-alerts-stored-in-the-event-hub"></a>Schritt 6: Konfigurieren der Splunk-Dateneingaben zum Verbrauchen von Sicherheitswarnungen, die im Event Hub gespeichert sind

Der letzte Schritt des Einrichtungsprozesses besteht darin, die Splunk-Dateneingaben so zu konfigurieren, dass sie den Event Hub, die Anwendung und die Geheimnisse nutzen, die Sie in den vorhergehenden Schritten erstellt haben.

1. Folgen Sie den Anweisungen im Thema [Splunk-Konfiguration](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Configuration-of-Splunk), um Splunk-Dateneingaben für das Azure Monitor-Add-On zu öffnen und zu konfigurieren. Wechseln Sie zu **Einstellungen** und **Dateneingaben**. Wählen Sie **Azure Monitor-Diagnoseprotokolle**.
2. Wählen Sie **Neu**, und füllen Sie alle erforderlichen Felder mit den Werten aus, die Sie in den vorhergehenden Schritten erhalten haben. Die folgende Abbildung zeigt alle erforderlichen Felder mit den Werten aus den vorherigen Beispielen in diesem Artikel.

    ![Azure Monitor Felder](images/azure-monitor-fields.png)

3. Wählen Sie **Weiter**, und suchen sie nach den Sicherheitswarnungen für Ihre Organisation, die von Azure Monitor abgerufen wurden.

## <a name="optional-use-splunk-search-to-explore-data"></a>(Optional) Untersuchen von Daten anhand der Splunk-Suche

Nachdem das Plug-in Azure Monitor Splunk eingerichtet haben, startet die Splunk-Instanz abrufen von Ereignissen aus der konfigurierten Ereignis bereit. Standardmäßig wird Splunk jede Eigenschaft des alert Microsoft Graph Sicherheit API-Schemas zum Zulassen der Suche indizieren.

Für die Suche nach Microsoft Graph Sicherheit API Benachrichtigungen, Dashboards erstellen oder Festlegen der Splunk Warnungen mit Ihrer Suchabfrage zu navigieren apps-Suche & Reporting-app in Splunk >.

**Beispiele**:<br/>
Suchen Sie Graph Sicherheitshinweise:

- Typ `sourcetype="amdl:securitygraph:alert"` bei der Suche angezeigt, die alle Benachrichtigungen erhalten möchten über die Sicherheit-API von Microsoft Graph verfügbar gemacht. Auf der rechten Seite sehen die Eigenschaften der obersten Ebene von Azure Monitor Protokoll Sie Eigenschaften dar, in dem Diagramm Sicherheitshinweis ist.<br/>
- Im linken Bereich sehen Sie die ausgewählten Felder und interessant. Können Sie ausgewählten Felder zum Erstellen von Dashboards oder Splunk Warnungen verwenden, können Sie auch hinzufügen oder ausgewählten Felder entfernen, indem Sie mit der rechten Maustaste auf die Felder.  
> **Hinweis:** Wie in der folgenden Abfrage gezeigt, können Sie die Suche einschränken, je nach Bedarf. Im Beispiel Filtern wir Sicherheitswarnungen Diagramm mithilfe von Azure Security Center hoher Schweregrad Benachrichtigungen. Wir auch verwendet `eventDatetime`, `severity`, `status`, und `provider` als ausgewählten Felder angezeigt werden sollen. Weitere Advance Suchbegriffe finden Sie unter [Search-Lernprogramme Splunk](https://docs.splunk.com/Documentation/Splunk/7.1.2/SearchTutorial/WelcometotheSearchTutorial).

 ![splunk_search_query](images/splunk-search-query.png)
> Suchabfrage:`sourcetype="amdl:securitygraph:alert" "properties.vendorInformation.provider"=ASC "properties.severity"=High | rename properties.eventDataTime as eventDateTime properties.severity as severity properties.vendorInformation.provider as provider properties.status as status`

Splunk kann auch mehrere Aktionen auf Suche Ergebnisse mit der Option "Speichern unter" im Menü in obere rechte Ecke des Bildschirms. Sie können Berichte, Dashboards Bereiche oder basierend auf Ihrer Suchfilter Benachrichtigungen erstellen.
Es folgt ein Beispiel für ein Dashboard mit eines Streams von Ereignissen auf der Grundlage der vorherigen Abfrage: Sie können jedes Ereignis Weitere Details auf Microsoft Graph-Website Zugriff auf einen Drilldown Link hinzufügen. Finden Sie unter [Splunk Drilldown-Dokumentation](https://docs.splunk.com/Documentation/Splunk/7.1.2/Viz/DrilldownIntro).

 ![splunk_search_results](images/splunk-search-results.png)

Oder Sie können ein Dashboard als ein Timeline-Diagramm erstellen:

 ![splunk_search_timeline](images/splunk-search-timeline.png)

Sie können [Splunk Search & Bericht Lernprogramm](https://docs.splunk.com/Documentation/Splunk/7.1.2/SearchTutorial/WelcometotheSearchTutorial) Einzelheiten folgen.

