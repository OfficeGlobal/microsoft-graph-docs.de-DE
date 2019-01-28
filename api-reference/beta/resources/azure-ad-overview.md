---
title: Arbeiten mit Azure Active Directory-Ressourcen in Microsoft Graph
description: Microsoft Graph für Azure Active Directory (Azure AD) bietet REST-APIs, die bei der Verwaltung Ihrer Organisation, Ressourcen und Objekte behilflich sind.
localization_priority: Priority
ms.openlocfilehash: 35e938caa05409cb7b4a9da66ef970f63685393c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512451"
---
# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>Arbeiten mit Azure Active Directory-Ressourcen in Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mit Microsoft Graph können Sie auf [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/active-directory-whatis)-Ressourcen zugreifen, um z. B. folgende Szenarios zu unterstützen: Verwalten von Administratorrollen (Verzeichnisrollen), Einladen von Benutzern, die nicht zu einer Organisation gehören, und als [Cloud-Lösungsanbieter (CSP)](https://partner.microsoft.com/cloud-solution-provider) auch Verwalten der Daten Ihrer Kunden. Microsoft Graph bietet auch Methoden, die Apps verwenden können, um beispielsweise Informationen zu den transitiven Gruppen- und Rollenmitgliedschaften von Benutzern zu ermitteln. 

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
| `directoryObject` ist die Basisklasse, von der viele Verzeichnisressourcen, z. B. Benutzer und Gruppen, erben. Microsoft Graph macht mehrere Methoden verfügbar, die Sie verwenden können, um Informationen über Benutzer, Gruppen und andere Verzeichnisobjekte zu ermitteln. Sie können beispielsweise eine transitive Mitgliedschaft in einer Liste von Gruppen überprüfen, alle Gruppen und Verzeichnisrollen zurückgeben, von denen ein Verzeichnisobjekt ein transitives Mitglied ist, oder alle Ressourcen eines bestimmten Typs (z. B. Benutzer oder Gruppe) aus einer Liste allgemeiner Ressourcen-IDs abrufen. | [directoryObject](../resources/directoryobject.md) | – |
| **Verwalten von Verzeichnisrollen (Administratorrollen), administrativen Einheiten, Verzeichniseinstellungen und Richtlinien** | | |
| Aktivieren Sie Verzeichnisrollen in einem Azure AD-Mandanten, und verwalten Sie Benutzermitgliedschaften in Verzeichnisrollen. Verzeichnisrollen werden auch als „Administratorrollen“ bezeichnet. | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) |[Zuweisen von Administratorrollen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)|
| Verwalten von administrativen Einheiten. Verzeichnisrollen delegieren ihren Mitgliedern mandantenweite Administratorrechte. Ein Administrator kann administrative Einheiten erstellen und verwalten, um Benutzern genauer begrenzte Administratorrechte zu delegieren. | [administrativeUnit](../resources/administrativeunit.md) | [Verwaltung von administrativen Einheiten in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-administrative-units-management) |
| Vordefinierte Verzeichniseinstellungen mandantenweit oder für einzelne Ressourceninstanzen anwenden. Derzeit werden nur die Einstellungen für Office 365-Gruppen unterstützt. Vordefinierte Gruppeneinstellungen mandantenweit oder für einzelne Ressourceninstanzen anwenden. Gruppeneinstellungen steuern Verhalten wie blockierte Wortlisten für Gruppenanzeigenamen, ob Gastbenutzer Gruppenbesitzer sein können und vieles mehr. | [directorySetting](../resources/directorysetting.md) <br/>[directorySettingTemplate](../resources/directorysettingtemplate.md)| [Azure Active Directory-Cmdlets für die Konfiguration von Gruppeneinstellungen](https://docs.microsoft.com/azure/active-directory/active-directory-accessmanagement-groups-settings-cmdlets)|
| Azure AD-Richtlinien auf Anwendungen, Dienstprinzipale, Gruppen oder auf die gesamte Organisation anwenden. Derzeit werden Richtlinien für die Tokenlebensdauer und die Startbereichsermittlung (Home Realm Discovery, HDR) unterstützt.  | [Richtlinie](../resources/policy.md) | – |
| **Schützen von privilegiertem Zugriff auf Azure AD** | | |
| Verwalten und überwachen des zeitgebundenen privilegierten Zugriff auf Verzeichnis- und Azure-Ressourcen für Administratoren und IT-Mitarbeiter mit Privileged Identity Management (PIM). | [Privileged Identity Management-APIs](../resources/privilegedidentitymanagement-root.md) | [Was ist Azure AD Privileged Identity Management?](https://docs.microsoft.com/azure/active-directory/active-directory-privileged-identity-management-configure)|
| Überwachen von Identitätsrisikoereignissen, z. B. dass sich Benutzer auf mit Schadsoftware infizierten Geräten oder von unüblichen Orten aus anmelden. | [Identity Protection-Dienst-API](../resources/identityprotection-root.md) | [Azure Active Directory Identity Protection](https://docs.microsoft.com/azure/active-directory/active-directory-identityprotection)<br/><br/>[Azure Active Directory-Risikoereignisse](https://docs.microsoft.com/de-DE/azure/active-directory/active-directory-reporting-risk-events) |
| **Verwalten von Geräten** | | |
| Verwalten Sie Geräte, die in der Organisation registriert sind. Geräte sind für Benutzer registriert und umfassen Elemente wie Laptops, Desktops, Tablets und Mobiltelefone. Geräte werden in der Regel mithilfe des Geräteregistrierungsdiensts oder von Microsoft Intune in der Cloud erstellt. Sie werden von Richtlinien für bedingten Zugriff für mehrstufige Authentifizierung verwendet. | [device](../resources/device.md) | [Erste Schritte bei der Azure Active Directory-Geräteregistrierung](https://docs.microsoft.com/azure/active-directory/active-directory-device-registration-overview)<br/><br/>[Was ist Intune?](https://docs.microsoft.com/intune-classic/understand-explore/introduction-to-microsoft-intune)<br/><br/>[Registrieren von Geräten für die Verwaltung in Intune](https://docs.microsoft.com/intune-classic/deploy-use/enroll-devices-in-microsoft-intune) |
| **App-Verwaltung** | | |
| Verwalten der App-Konfiguration in einem Entwicklermandanten. | [application](../resources/application.md) | [Anwendungs- und Dienstprinzipalobjekte in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| Verwalten der auf einem Mandanten installierten Apps. | [servicePrinicpal](../resources/serviceprincipal.md) | [Anwendungs- und Dienstprinzipalobjekte in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-application-objects) |
| Verwalten von Berechtigungen, die von Benutzern und Administratoren genehmigt wurden, in Apps, die auf einem Mandanten installiert sind. | [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) | – |
| Verwalten von Benutzer-, Gruppen- und Dienstprinzipal-Rollenmitgliedschaften in Apps, die auf einem Mandanten installiert sind. | [appRoleAssignment](../resources/approleassignment.md) | – |
| **Verwaltung von Partnermandanten** | | |
| Abrufen von Informationen über Partnerschaften mit Kundenmandanten. <br/><br/>**Hinweis:** Dies gilt nur für Partnermandanten. Partnermandanten sind Azure AD-Mandanten, die zu Microsoft-Partnern gehören, die Teil der Partnerprogramme [Microsoft Cloud-Lösungsanbieter](https://partnercenter.microsoft.com/partner/programs), Office 365 Syndication oder Microsoft Advisor sind.| [contract](../resources/contract.md) | [Aufrufen von Microsoft Graph aus einer Anwendung eines Cloud-Lösungsanbieters](/graph/auth-cloudsolutionprovider) |
| Verwalten von Domänen, die einem Mandanten zugeordnet sind. Mithilfe von Domänenvorgängen können Registrierungsstellen die Domänenzuweisung für Dienste wie Office 365 automatisieren. | [domain](../resources/domain.md) | [Hinzufügen eines benutzerdefinierten Domänennamens zu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-domains-add-azure-portal) |
| **Verwaltung von Mandanten** | | |
| Rufen Sie Informationen über eine Organisation ab, z. B. die Unternehmensadresse, Kontakte für technische Fragen und Benachrichtigungen, die Dienstpläne, die die Organisation abonniert hat, sowie die Domänen, die mit dieser verknüpft sind. | [organization](../resources/organization.md) | Nicht zutreffend |
| Ruft Informationen zu den Dienst-SKUs ab, die ein Unternehmen abonniert hat. | [subscribedSku](../resources/subscribedsku.md) | Nicht zutreffend |
| Einladen externer (Gast)Benutzer zu einer Organisation. | [invitation](../resources/invitation.md) | [Was ist die Azure AD B2B-Zusammenarbeit?](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b)|
| **Zugriffsüberprüfungen** | | |
| Überprüfen Sie mit Zugriffsüberprüfungen, dass Gruppenmitgliedschaften und Zugriffsrechte für die Anwendung korrekt sind. | [Zugriffsüberprüfungs-API](../resources/accessreviews-root.md) |[Zugriffsüberprüfungen in Azure AD](https://docs.microsoft.com/de-DE/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) |
## <a name="next-steps"></a>Nächste Schritte
Verzeichnisressourcen und APIs können Ihnen neue Möglichkeiten eröffnen, über die Sie mit Benutzer in Kontakt treten und ihre Erfahrungen mit Microsoft Graph verwalten können. So erhalten Sie weitere Informationen: 

- Informieren Sie sich ausführlicher über die Methoden und Eigenschaften der Ressourcen, die für Ihr Szenario am hilfreichsten sind.
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.

Benötigen Sie weitere Ideen? Dann sehen Sie sich an, [wie unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/graph/graph/examples#partners).

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/azure-ad-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
