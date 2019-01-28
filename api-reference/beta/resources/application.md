---
title: application-Ressourcentyp
description: 'Steht für eine Anwendung. Jede Anwendung, bei der die Authentifizierung mit Azure Active Directory (Azure AD) erfolgt, muss in einem Verzeichnis registriert werden. Bei der Anwendungsregistrierung erhält Azure AD Informationen über Ihre Anwendung, darunter die URL, unter der sich die Anwendung befindet, die URL, an die Antworten nach Authentifizierung gesendet werden, der URI zum Identifizieren der Anwendung und mehr. Weitere Informationen finden Sie unter „Grundlegendes zur Registrierung einer Anwendung in Azure AD“. Erbt von directoryObject. '
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 694f6b12dd8fe1fd59f12cafebd47c842a4077cb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529222"
---
# <a name="application-resource-type"></a>application-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Steht für eine Anwendung. Jede Anwendung, bei der die Authentifizierung mit Azure Active Directory (Azure AD) erfolgt, muss in einem Verzeichnis registriert werden. Bei der Anwendungsregistrierung erhält Azure AD Informationen über Ihre Anwendung, darunter die URL, unter der sich die Anwendung befindet, die URL, an die Antworten nach Authentifizierung gesendet werden, der URI zum Identifizieren der Anwendung und mehr. Weitere Informationen finden Sie unter [Grundlegendes zur Registrierung einer Anwendung in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad). Erbt von [directoryObject](directoryobject.md). 

> **Hinweis:** Änderungen an dem application-Ressourcentyp befinden sich derzeit in der Entwicklung. Weitere Informationen finden Sie unter [Bekannte Probleme in Microsoft Graph](/graph/known-issues#application-and-serviceprincipal-api-changes).

Diese Ressource unterstützt Folgendes:

- Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/application-delta.md)-Funktion.

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:---------------|:--------|:----------|
|[Get application](../api/application-get.md) | Anwendung |Dient zum Lesen der Eigenschaften und der Beziehungen des Anwendungsobjekts.|
|[Create application](../api/application-post-applications.md) | Anwendung | Erstellt (registriert) eine neue Anwendung.|
|[List applications](../api/application-list.md) | Anwendung | Dient zum Abrufen der Liste von Anwendungen in der Organisation. |
|[Update application](../api/application-update.md) | Anwendung |Dient zum Aktualisieren des Anwendungsobjekts. |
|[Delete application](../api/application-delete.md) | Keine |Dient zum Löschen des Anwendungsobjekts. |
|[List assigned policies](../api/policy-list-assigned.md)| [policy](policy.md)-Sammlung| Abrufen aller diesem Objekt zugewiesener Richtlinien.|
|[Create owner](../api/application-post-owners.md) |[directoryObject](directoryobject.md)| Dient zum Erstellen eines neuen Besitzers durch Veröffentlichen in der Benutzersammlung.|
|[List owners](../api/application-list-owners.md) |[directoryObject](directoryobject.md)-Sammlung| Dient zum Abrufen einer Besitzerobjektsammlung.|
|[delta](../api/application-delta.md)|application-Sammlung| Ruft inkrementelle Änderungen für Anwendungen ab. |
|[Create call](../api/application-post-calls.md)|[call](call.md)|Dient zum Erstellen eines neuen Aufrufs durch Veröffentlichen in der Aufrufsammlung.|
|[Create online meeting](../api/application-post-onlinemeetings.md)|[onlineMeeting](onlinemeeting.md)|Dient zum Erstellen einer neuen Onlinebesprechung durch Veröffentlichen in der onlineMeetings-Sammlung.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|api|[api](api.md)| Legt die Einstellungen für eine API-Anwendung fest. |
|appId| String | Der eindeutige Bezeichner für die Anwendung, der einer Anwendung durch Azure AD zugewiesen ist. Lässt keine Nullwerte zu. Schreibgeschützt. |
|appRoles|[appRole](approle.md)-Sammlung|Die Sammlung der Anwendungsrollen, die eine Anwendung möglicherweise deklariert. Diese Rollen können Benutzern, Gruppen oder Dienstprinzipalen zugewiesen werden. Lässt keine Nullwerte zu.|
|createdDateTime|DateTimeOffset| Datum und Uhrzeit der Anwendungsregistrierung. |
|deletedDateTime|DateTimeOffset| Datum und Uhrzeit der Anwendungslöschung. |
|displayName|String|Der Anzeigename der Anwendung. |
|id|String|Eindeutiger Bezeichner für die Anwendung. Geerbt von [directoryObject](directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt. |
|identifierUris|String-Sammlung| Die URIs, die die Anwendung identifizieren. Weitere Informationen finden Sie unter [Anwendungsobjekte und Dienstprinzipalobjekte](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/). Der *any*-Operator ist für Filterausdrücke für mehrwertige Eigenschaften erforderlich. Lässt keine Nullwerte zu. |
|info|[informationalUrl](informationalurl.md)| Grundlegende Profilinformationen der Anwendung. |
|isFallbackPublicClient|Boolesch| Legt den Fallback-App-Typ auf öffentlichen Client fest, z. B. eine installierte App, die auf einem mobilen Gerät ausgeführt wird. Der Standardwert ist *false*, d. h. der Fallback-App-Typ ist vertraulicher Client, zum Beispiel Web-App. Bei einigen Szenarien kann Azure AD den Client-App-Typ nicht ermitteln (z. B. [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3)-Fluss, wo dieser ohne Angabe eines Umleitungs-URIs konfiguriert ist). In diesen Fällen interpretiert Azure AD den App-Typ basierend auf dem Wert dieser Eigenschaft.|
|keyCredentials|[keyCredential](keycredential.md)-Sammlung|Die Sammlung der wichtigsten Anmeldeinformationen, die mit der Anwendung verknüpft sind. Lässt keine Nullwerte zu. |
|logo|Stream|Das Hauptlogo für die Anwendung. Lässt keine Nullwerte zu. |
|optionalClaims|optionalClaims| Reserviert für zukünftige Verwendung. |
|orgRestrictions|String-Sammlung| Reserviert für zukünftige Verwendung. |
|parentalControlSettings|[parentalControlSettings](parentalcontrolsettings.md) |Gibt die Jugendschutzeinstellungen für eine Anwendung an.|
|passwordCredentials|[passwordCredential](passwordcredential.md)-Sammlung|Die Sammlung der Kennwortanmeldeinformationen, die mit der Anwendung verknüpft sind. Lässt keine Nullwerte zu.|
|publicClient|[publicClient](publicclient.md)| Legt die Einstellungen für installierte Clients wie Desktop- oder mobile Geräte fest. |
|publisherDomain| String | Die bestätigte Herausgeberdomäne für die Anwendung. Schreibgeschützt.|
|requiredResourceAccess|[requiredResourceAccess](requiredresourceaccess.md)-Sammlung|Gibt Ressourcen an, auf die diese Anwendung zugreifen muss, sowie den Satz von OAuth-Berechtigungsbereichen und Anwendungsrollen, die unter den jeweiligen Ressourcen benötigt werden. Durch diese Vorkonfiguration des erforderlichen Ressourcenzugriffs wird die Zustimmungsoberfläche bestimmt. Lässt keine Nullwerte zu.|
|signInAudience | String | Gibt an, welche Microsoft-Konten für die aktuelle Anwendung unterstützt werden. Unterstützte Werte:<ul><li>**AzureADMyOrg**: Benutzer mit einem Microsoft-Geschäfts-, Schul- oder Unikonto in dem Azure AD-Mandanten meiner Organisation (d. h. einzelner Mandant).</li><li>**AzureADMultipleOrgs**: Benutzer mit einem Microsoft-Geschäfts-, Schul- oder Unikonto in dem Azure AD-Mandanten einer Organisation (d. h. mehrere Mandanten).</li> <li>**AzureADandPersonalMicrosoftAccount**: Benutzer mit einem persönlichen Microsoft-Konto oder einem Geschäfts-, Schul- oder Unikonto im Azure AD-Mandanten einer Organisation.</li></ul> | `AzureADandPersonalMicrosoftAccount` |
|tags|String-Sammlung| Benutzerdefinierte Zeichenfolgen, die zum Kategorisieren und Identifizieren der Anwendung verwendet werden können. |
|web|[web](web.md)| Legt die Einstellungen für eine Webanwendung fest. |

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ | Beschreibung |
|:---------------|:--------|:----------|
|Aufrufe           |[call](call.md)-Sammlung                  |Schreibgeschützt. Lässt Nullwerte zu.|
|connectorGroup|[connectorGroup](connectorgroup.md)| Das connectorGroup-Objekt, das die Anwendung mit dem Azure AD-Anwendungsproxy verwendet. Lässt Nullwerte zu.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Schreibgeschützt.|
|onlineMeetings  |[onlineMeeting](onlinemeeting.md)-Sammlung|Schreibgeschützt. Lässt Nullwerte zu.|
|Besitzer|[directoryObject](directoryobject.md)-Sammlung|Verzeichnisobjekte, die Besitzer der Anwendung sind. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind und die berechtigt sind, dieses Objekt zu ändern. Version vom 08.11.2013 oder neuer erforderlich. Schreibgeschützt. Lässt Nullwerte zu.|
|Richtlinie|[policy](policy.md)-Sammlung|Die dieser Anwendung zugewiesenen Richtlinien.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "createdOnBehalfOf",
    "owners"
  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "api": {"@odata.type": "microsoft.graph.apiApplication"},
  "appId": "String",
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "identifierUris": ["String"],
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "isFallbackPublicClient": true,
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logo": "Stream",
  "optionalClaims": [{"@odata.type": "microsoft.graph.optionalClaims"}],
  "orgRestrictions": ["Guid"],
  "parentalControlSettings": [{"@odata.type": "microsoft.graph.parentalControlSettings"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "preAuthorizedApplications": [{"@odata.type": "microsoft.graph.preAuthorizedApplication"}],
  "publicClient": {"@odata.type": "microsoft.graph.publicClientApplication"},
  "publisherDomain": "String",
  "requiredResourceAccess": [{"@odata.type": "microsoft.graph.requiredResourceAccess"}],
  "signInAudience": "String",
  "tags": ["String"],
  "web": {"@odata.type": "microsoft.graph.webApplication"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/application.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
