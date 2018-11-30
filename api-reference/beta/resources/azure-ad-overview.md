---
title: Arbeiten mit Azure Active Directory-Ressourcen in Microsoft Graph
description: 'Mit Microsoft Graph können Sie zugreifen, Azure Active Directory (AD Azure) Ressourcen zum Aktivieren von Szenarien wie verwalten Administratorrollen (Directory), externe Benutzer zu einer Organisation einladen, und, wenn Sie einen Cloud Lösung (CSP) sind, Ihre Kundendaten. Microsoft Graph bietet auch Methoden apps verwenden können, beispielsweise zum Ermitteln von Informationen über Benutzer transitiven Gruppe und Rollenmitgliedschaften. '
ms.openlocfilehash: 4f33004e5bacf71c2e7cd3af5bad78448983dec7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066031"
---
# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>Arbeiten mit Azure Active Directory-Ressourcen in Microsoft Graph

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Mit Microsoft Graph Sie [Azure Active Directory (AD Azure)](https://docs.microsoft.com/azure/active-directory/active-directory-whatis) auf Ressourcen zugreifen können zum Aktivieren von Szenarien wie das Verwalten von Administratorrollen (Directory) einladen von externen Benutzern einer Organisation und, wenn Sie eine [Cloud-Lösung Provider (CSP)](https://partner.microsoft.com/cloud-solution-provider)sind Verwalten von Daten des Kunden. Microsoft Graph bietet auch Methoden apps verwenden können, beispielsweise zum Ermitteln von Informationen über Benutzer transitiven Gruppe und Rollenmitgliedschaften. 

> **Hinweis**: Einige Azure AD-Ressourcen sind in anderen Abschnitten der API-Referenz dokumentiert. Weitere Informationen finden Sie unter [Benutzer](users.md) und [Gruppen](group.md).


## <a name="authorization"></a>Authorization
 
Zum Aufrufen der Microsoft Graph-APIs in Azure AD-Ressourcen benötigt Ihre App die entsprechenden Berechtigungen. Viele der APIs, die in Azure AD-Ressourcen verfügbar gemacht werden, erfordern eine der [ _Verzeichnis_berechtigungen](/graph/permissions-reference#directory-permissions). Verzeichnisberechtigungen verfügen über hohe Rechte und müssen immer vom Administrator genehmigt werden. 

Wenn Ihre App im Namen eines Benutzers agiert (delegierte Berechtigungen), muss dieser Benutzer ein Mitglied einer entsprechenden [Administratorrolle](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles) sein, damit Ihre App viele der Azure AD-APIs erfolgreich aufrufen kann.

Weitere Informationen zu Berechtigungen, einschließlich delegierten und Anwendungsberechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference). 

## <a name="common-use-cases"></a>Allgemeine Anwendungsfälle 

In der folgenden Tabelle werden einige häufige Anwendungsfälle für Azure AD-Ressourcen aufgelistet.

| **Anwendungsfälle**        | **REST-Ressourcen** | **Siehe auch** |
|:-----------------|:--------|:----------|
| **Verzeichnisobjekt und Methoden** | | |
| `directoryObject` ist die Basisklasse, von der viele Verzeichnisressourcen, z. B. Benutzer und Gruppen, erben. Microsoft Graph macht mehrere Methoden verfügbar, die Sie verwenden können, um Informationen über Benutzer, Gruppen und andere Verzeichnisobjekte zu ermitteln. Sie können beispielsweise eine transitive Mitgliedschaft in einer Liste von Gruppen überprüfen, alle Gruppen und Verzeichnisrollen zurückgeben, von denen ein Verzeichnisobjekt ein transitives Mitglied ist, oder alle Ressourcen eines bestimmten Typs (z. B. Benutzer oder Gruppe) aus einer Liste allgemeiner Ressourcen-IDs abrufen. | [directoryObject](../resources/directoryobject.md) | Nicht zutreffend |
| **Verwalten von Rollen Verzeichnis (Administrator), administrativen Einheiten, Directory-Einstellungen und Richtlinie** | | |
| Aktivieren Sie Verzeichnisrollen in einem Azure AD-Mandanten, und verwalten Sie Benutzermitgliedschaften in Verzeichnisrollen. Verzeichnisrollen werden auch als „Administratorrollen“ bezeichnet. | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) |[Zuweisen von Administratorrollen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)|
| Verwalten von administrativen Einheiten. Verzeichnis Rollen Autorität Mandanten geltende von ihren Mitglieder. Ein Administrator kann erstellen und Verwalten von administrativen Einheiten um genauer gesagt bereichsbezogenen an Benutzer delegieren. | [administrativeUnit](../resources/administrativeunit.md) | [Administrative Einheiten Management in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-administrative-units-management) |
| Vordefinierte Directory-Einstellungen über einen Mandanten oder für einzelne Ressourceninstanzen anwenden. Derzeit werden nur Einstellungen für Office 365-Gruppen unterstützt. Directory Einstellungen Steuerelementverhalten wie blockierte Word Listen für den Anzeigenamen, die Gruppe, ob Gastbenutzer Gruppenbesitzer und vieles mehr werden dürfen. | [Verzeichnisberechtigungen](../resources/directorysetting.md) <br/>[directorySettingTemplate](../resources/directorysettingtemplate.md)| [Azure Active Directory-Cmdlets für die Konfiguration von Gruppeneinstellungen](https://docs.microsoft.com/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| Anwenden von Azure AD-Richtlinien auf Applications, Dienstprinzipale, Gruppen oder die gesamte Organisation. Derzeit werden Richtlinien für die Gültigkeitsdauer von token und Startbereichs-Suche unterstützt.  | [Richtlinie](../resources/policy.md) | Nicht zutreffend |
| **Sichere Systemzugriff Azure AD** | | |
| Verwalten und Überwachen von Zeit gebundene Systemzugriff Verzeichnis und Azure Ressourcen für Administratoren und IT-Spezialisten mit privilegierten Identity Management (PIM). | [Privilegierten Identitätsmanagement-API](../resources/privilegedidentitymanagement-root.md) | [Was ist Azure AD privilegierten Identitätsmanagement?](https://docs.microsoft.com/azure/active-directory/active-directory-privileged-identity-management-configure)|
| Überwachen von Ereignissen Identität Risiko wie Benutzer anmelden von Schadsoftware infiziert Geräte oder Speicherorte nicht vertraut. | [Identität Protection-Dienst-API](../resources/identityprotection-root.md) | [Azure Active Directory-Schutz](https://docs.microsoft.com/azure/active-directory/active-directory-identityprotection)<br/><br/>[Azure Active Directory Risiko-Ereignisse](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events) |
| **Verwalten von Geräten** | | |
| Verwalten Sie Geräte, die in der Organisation registriert sind. Geräte sind für Benutzer registriert und umfassen Elemente wie Laptops, Desktops, Tablets und Mobiltelefone. Geräte werden in der Regel mithilfe des Geräteregistrierungsdiensts oder von Microsoft Intune in der Cloud erstellt. Sie werden von Richtlinien für bedingten Zugriff für mehrstufige Authentifizierung verwendet. | [device](../resources/device.md) | [Erste Schritte mit Azure Active Directory-Gerät-Registrierung](https://docs.microsoft.com/azure/active-directory/active-directory-device-registration-overview)<br/><br/>[Was ist Intune?](https://docs.microsoft.com/intune-classic/understand-explore/introduction-to-microsoft-intune)<br/><br/>[Registrieren von Geräten für die Verwaltung in Intune](https://docs.microsoft.com/intune-classic/deploy-use/enroll-devices-in-microsoft-intune) |
| **App-Verwaltung** | | |
| Verwalten von app-Konfiguration in einem Entwickler-Mandanten. | [application](../resources/application.md) | [Anwendung und Service principal-Objekten in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| Verwalten von apps in einem Mandanten installiert. | [servicePrinicpal](../resources/serviceprincipal.md) | [Anwendung und Service principal-Objekten in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| Verwalten von Berechtigungen von Benutzern und Administratoren für apps in einem Mandanten installiert zugestimmt. | [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) | Nicht zutreffend |
| Verwalten von Benutzern, Gruppen und Service principal Rollenmitgliedschaften auf apps in einem Mandanten installiert. | [appRoleAssignment](../resources/approleassignment.md) | Nicht zutreffend |
| **Verwaltung von Partnermandanten** | | |
| Abrufen von Informationen über Partnerschaften mit Kundenmandanten. <br/><br/>**Hinweis:** Dies gilt nur für Partnermandanten. Partnermandanten sind Azure AD-Mandanten, die zu Microsoft-Partnern gehören, die Teil der Partnerprogramme [Microsoft Cloud-Lösungsanbieter](https://partnercenter.microsoft.com/partner/programs), Office 365 Syndication oder Microsoft Advisor sind.| [contract](../resources/contract.md) | [Aufrufen von Microsoft Graph aus einer Anwendung eines Cloud-Lösungsanbieters](/graph/auth-cloudsolutionprovider) |
| Verwalten von Domänen, die einem Mandanten zugeordnet sind. Mithilfe von Domänenvorgängen können Registrierungsstellen die Domänenzuweisung für Dienste wie Office 365 automatisieren. | [domain](../resources/domain.md) | [Hinzufügen eines benutzerdefinierten Domänennamens zu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-domains-add-azure-portal) |
| **Verwaltung von Mandanten** | | |
| Rufen Sie Informationen über eine Organisation ab, z. B. die Unternehmensadresse, Kontakte für technische Fragen und Benachrichtigungen, die Dienstpläne, die die Organisation abonniert hat, sowie die Domänen, die mit dieser verknüpft sind. | [organization](../resources/organization.md) | Nicht zutreffend |
| Ruft Informationen zu den Dienst-SKUs ab, die ein Unternehmen abonniert hat. | [subscribedSku](../resources/subscribedsku.md) | Nicht zutreffend |
| Einladen externer (Gast)Benutzer zu einer Organisation. | [invitation](../resources/invitation.md) | [Was ist die Azure AD B2B-Zusammenarbeit?](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b)|
| **Access Reviews (engl.)** | | |
| Stellen Sie sicher, Gruppenmitgliedschaften und Zugriffsrechte für die Anwendung mit Access Bewertungen richtig sind | [Access überprüft API](../resources/accessreviews-root.md) |[Prüft Azure AD-Zugriff](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) |
## <a name="next-steps"></a>Nächste Schritte
Verzeichnisressourcen und APIs können Ihnen neue Möglichkeiten eröffnen, über die Sie mit Benutzer in Kontakt treten und ihre Erfahrungen mit Microsoft Graph verwalten können. So erhalten Sie weitere Informationen: 

- Informieren Sie sich ausführlicher über die Methoden und Eigenschaften der Ressourcen, die für Ihr Szenario am hilfreichsten sind.
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.

Benötigen Sie weitere Ideen? Dann sehen Sie sich an, [wie unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/graph/graph/examples#partners).

