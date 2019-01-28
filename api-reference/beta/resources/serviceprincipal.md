---
title: servicePrincipal-Ressourcentyp
description: Stellt eine Instanz einer Anwendung in einem Verzeichnis dar. Erbt von directoryObject.
localization_priority: Priority
ms.openlocfilehash: d36a82ae885725387e788cf280442afe09fa63de
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574187"
---
# <a name="serviceprincipal-resource-type"></a>servicePrincipal-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Instanz einer Anwendung in einem Verzeichnis dar. Erbt von [directoryObject](directoryobject.md).

Diese Ressource unterstützt Folgendes:

- Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/serviceprincipal-delta.md)-Funktion.

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "appRoleAssignedTo",
    "appRoleAssignments",
    "createdObjects",
    "createdOnBehalfOf",
    "memberOf",
    "oauth2PermissionGrants",
    "ownedObjects",
    "owners"
  ],
  "@odata.type": "microsoft.graph.servicePrincipal"
}-->

```json
{
  "accountEnabled": true,
  "addIns": [{"@odata.type": "microsoft.graph.addIn"}],
  "appDisplayName": "string",
  "appId": "string",
  "appOwnerOrganizationId": "guid",
  "appRoleAssignmentRequired": true,
  "displayName": "string",
  "errorUrl": "string",
  "homepage": "string",
  "id": "string (identifier)",
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logoutUrl": "string",
  "oauth2Permissions": [{"@odata.type": "microsoft.graph.oAuth2Permission"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "preferredTokenSigningKeyThumbprint": "string",
  "publisherName": "string",
  "replyUrls": ["string"],
  "samlMetadataUrl": "string",
  "servicePrincipalNames": ["string"],
  "tags": ["string"]
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ |Beschreibung|
|:---------------|:--------|:----------|
|accountEnabled|Boolescher Wert| **True**, wenn das Dienstprinzipalkonto aktiviert ist; andernfalls **false**.            |
|appDisplayName|Zeichenfolge|Der von der verknüpften Anwendung verfügbar gemachte Anzeigename.|
|appId|Zeichenfolge|Die eindeutige ID für die verknüpfte Anwendung (die **appId**-Eigenschaft).|
|appRoleAssignmentRequired|Boolescher Wert|Gibt an, ob eine **eppRoleAssignment** für einen Benutzer oder eine Gruppe erforderlichist, bevor Azure Active Directory ein Benutzer- oder Zugriffstoken für die Anwendung ausstellt. Lässt keine Nullwerte zu. |
|appRoles|[appRole](approle.md)-Auflistung|Die von der verknüpften Anwendung verfügbar gemachten Anwendungsrollen. Weitere Informationen finden Sie in der **appRoles**-Eigenschaftsdefinition in der [application](application.md)-Entität. Lässt keine Nullwerte zu. |
|displayName|Zeichenfolge|Der Anzeigename für den Dienstprinzipal.|
|errorUrl|Zeichenfolge|            |
|homepage|Zeichenfolge|Die URL für die Startseite der verknüpften Anwendung.|
|keyCredentials|[keyCredential](keycredential.md)-Auflistung|Die Auflistung der wichtigsten Anmeldeinformationen, die mit dem Dienstprinzipal verknüpft sind. Lässt keine Nullwerte zu.            |
|logoutUrl|Zeichenfolge| Gibt die URL an, die vom Autorisierungsdienst von Microsoft verwendet wird, um einen Benutzer mithilfe von [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html)-, [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html)- oder SAML-Abmeldeprotokollen abzumelden.  |
|oauth2Permissions|[oAuth2Permission](oauth2permission.md)-Auflistung|Die von der verknüpften Anwendung verfügbar gemachten OAuth 2.0-Berechtigungen. Weitere Informationen finden Sie in der **oauth2Permissions**-Eigenschaftsdefinition in der [application](application.md)-Entität. Lässt keine Nullwerte zu.            |
|id|Zeichenfolge|Der eindeutige Bezeichner für den Dienstprinzipal. Geerbt von [directoryObject](directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt.|
|passwordCredentials|[passwordCredential](passwordcredential.md)-Auflistung|Die Auflistung der Kennwortanmeldeinformationen, die mit dem Dienstprinzipal verknüpft sind. Lässt keine Nullwerte zu. |
|preferredTokenSigningKeyThumbprint|Zeichenfolge|Nur für die interne Verwendung reserviert. Schreiben Sie diese Eigenschaft nicht, und verwenden Sie diese Eigenschaft nicht anderweitig. Sie kann in zukünftigen Versionen möglicherweise entfernt werden. |
|publisherName|Zeichenfolge|Der Anzeigename des Mandanten, in dem verknüpfte Anwendung angegeben wird.|
|replyUrls|Zeichenfolgenauflistung|Die URLs, an die Benutzertoken zur Anmeldung bei der verknüpften Anwendung gesendet werden, oder die Umleitungs-URIs, an die die OAuth 2.0-Autorisierungscodes und Zugriffstoken für die verknüpfte Anwendung gesendet werden. Lässt keine Nullwerte zu. |
|samlMetadataUrl|Zeichenfolge| |
|servicePrincipalNames|Zeichenfolgenauflistung|Die URLs, die die verknüpfte Anwendung identifizieren. Weitere Informationen finden Sie unter [Anwendungs- und Dienstprinzipalobjekte](https://msdn.microsoft.com/library/azure/dn132633.aspx). Der **any**-Operator ist für Filterausdrücke in mehrwertigen Eigenschaften erforderlich.  Lässt keine Nullwerte zu. |
|tags|Zeichenfolgenauflistung| Lässt keine Nullwerte zu. |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ |Beschreibung|
|:---------------|:--------|:----------|
|appRoleAssignedTo| [appRoleAssignment](approleassignment.md) |Prinzipale (Benutzer, Gruppen und Dienstprinzipale), die diesem Dienstprinzipal zugewiesen sind. Schreibgeschützt.|
|appRoleAssignments|[appRoleAssignment](approleassignment.md)-Auflistung|Anwendungen, denen der Dienstprinzipal zugewiesen ist. Schreibgeschützt. Lässt NULL-Werte zu.|
|createdObjects|[directoryObject](directoryobject.md)-Sammlung|Verzeichnisobjekte, die von diesem Dienstprinzipal erstellt werden. Schreibgeschützt. Lässt Nullwerte zu.|
|memberOf| [directoryObject](directoryobject.md)-Sammlung|Rollen, denen dieser Dienstprinzipal angehört. HTTP-Methoden: GET; schreibgeschützt. Nullwerte zulassend.|
|oauth2PermissionGrants| [oAuth2PermissionGrant](oauth2permissiongrant.md)-Auflistung|Gewährungen für den Identitätswechsel von Benutzern, die diesem Dienstprinzipal zugewiesen sind. Schreibgeschützt. Lässt NULL-Werte zu.|
|ownedObjects| [directoryObject](directoryobject.md)-Sammlung|Verzeichnisobjekte, die im Besitz dieses Dienstprinzipals sind. Schreibgeschützt. Nullwerte zulassend.|
|owners| [directoryObject](directoryobject.md)-Sammlung|Verzeichnisobjekte, die Besitzer dieses Dienstprinzipals sind. Bei den Besitzern handelt es sich um eine Reihe von Benutzern, die keine Administratoren sind und die berechtigt sind, dieses Objekt zu ändern. Schreibgeschützt. Nullwerte zulassend.|
|policy| [policy](policy.md)-Auflistung|Die diesem Dienstprinzipal zugewiesenen Richtlinien.|

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Get servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |Dient zum Lesen der Eigenschaften und Beziehungen des servicePrincipal-Objekts.|
|[List servicePrincipals](../api/serviceprincipal-list.md) | [servicePrincipal](serviceprincipal.md)-Auflistung | Abrufen einer Liste von servicePrincipal-Objekten. |
|[Create appRoleAssignment](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| Erstellen einer neuen appRoleAssignment durch Veröffentlichen in der appRoleAssignments-Auflistung.|
|[List appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |[appRoleAssignment](approleassignment.md)-Auflistung| Abrufen einer appRoleAssignment-Objektauflistung.|
|[List createdObjects](../api/serviceprincipal-list-createdobjects.md) |[directoryObject](directoryobject.md)-Sammlung| Abrufen einer createdObject-Objektauflistung.|
|[List memberOf](../api/serviceprincipal-list-memberof.md) |[directoryObject](directoryobject.md)-Sammlung| Ruft die Gruppen, bei denen dieser Dienstprinzipal direktes Mitglied ist, aus der memberOf-Navigationseigenschaft ab.|
|[List transitive memberOf](../api/serviceprincipal-list-transitivememberof.md) |[directoryObject](directoryobject.md)-Sammlung| Auflisten der Gruppen, denen dieser Dienstprinzipal angehört. Dieser Vorgang ist transitiv und schließt die Gruppen ein, in denen dieser Dienstprinzipal ein geschachteltes Mitglied. |
|[List assigned policies](../api/policy-list-assigned.md)| [policy](policy.md)-Auflistung| Abrufen aller diesem Objekt zugewiesene Richtlinien.|
|[List oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |[oAuth2PermissionGrant](oauth2permissiongrant.md)-Auflistung| Abrufen einer oAuth2PermissionGrant-Objektauflistung.|
|[List ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |[directoryObject](directoryobject.md)-Sammlung| Abrufen einer ownedObject-Objektauflistung.|
|[Add owner](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| Dient zum Erstellen eines neuen Besitzers durch Veröffentlichen in der Benutzersammlung.|
|[List owners](../api/serviceprincipal-list-owners.md) |[directoryObject](directoryobject.md)-Sammlung| Dient zum Abrufen einer Besitzerobjektsammlung.|
|[Update](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |Aktualisieren des servicePrincipal-Objekts. |
|[Delete](../api/serviceprincipal-delete.md) | Keine |Löschen des servicePrincipal-Objekts. |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|Zeichenfolgenauflistung||
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|Zeichenfolgenauflistung||
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|Zeichenfolgenauflistung||
|[delta](../api/serviceprincipal-delta.md)|servicePrincipal-Auflistung| Ruft inkrementelle Änderungen für Dienstprinzipale ab. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/serviceprincipal.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
