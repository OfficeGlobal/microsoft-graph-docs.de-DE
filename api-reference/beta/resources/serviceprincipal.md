---
title: Ressourcentyp servicePrincipal
description: Stellt eine Instanz einer Anwendung in einem Verzeichnis. Erbt von directoryObject.
localization_priority: Priority
ms.openlocfilehash: 2df27225f62e7c2b7b026bb3d829abf546241267
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880206"
---
# <a name="serviceprincipal-resource-type"></a>Ressourcentyp servicePrincipal

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Instanz einer Anwendung in einem Verzeichnis. Erbt von [directoryObject](directoryobject.md).

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
  "@odata.type": "microsoft.graph.serviceprincipal"
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
|accountEnabled|Boolescher Wert| **true,** Wenn das Dienstkonto für den Prinzipal aktiviert ist. anderenfalls **false**.            |
|appDisplayName|Zeichenfolge|Der Anzeigename, der von der zugeordneten Anwendung verfügbar gemacht werden.|
|appId|Zeichenfolge|Der eindeutige Bezeichner für die zugewiesene Anwendung (dessen **AppId** -Eigenschaft).|
|appRoleAssignmentRequired|Boolescher Wert|Gibt an, ob ein **AppRoleAssignment** für einen Benutzer oder Gruppe erforderlich ist, bevor Azure AD einen Benutzer oder eine Zugriffstoken an die Anwendung ausstellt. Lässt keine Nullwerte zu. |
|appRoles|[AppRole](approle.md) -Auflistung|Die Rollen der Anwendung von der zugeordneten Anwendung verfügbar gemacht werden. Weitere Informationen finden Sie in der Definition der **AppRoles** -Eigenschaft in der [Anwendung](application.md) Entität. Lässt keine Nullwerte zu. |
|displayName|Zeichenfolge|Der Anzeigename für den Dienstprinzipal.|
|errorUrl|Zeichenfolge|            |
|Homepage|Zeichenfolge|Die URL zur Homepage der zugehörigen Anwendung.|
|keyCredentials|[KeyCredential](keycredential.md) -Auflistung|Die Auflistung von wichtigen Anmeldeinformationen, die dem Prinzipal Dienst zugeordnet sind. Lässt keine Nullwerte zu.            |
|logoutUrl|Zeichenfolge| Gibt die URL, die von Microsoft Autorisierungsdienst Abmelden ein Benutzer mit der [Vorderseite-Kanal](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [Back-Kanal](https://openid.net/specs/openid-connect-backchannel-1_0.html) oder SAML Abmeldung Protokolle verwendet werden soll.  |
|oauth2Permissions|[oAuth2Permission](oauth2permission.md) -Auflistung|Die OAuth 2.0-Berechtigungen von der zugeordneten Anwendung verfügbar gemacht werden. Weitere Informationen finden Sie in der Definition der **oauth2Permissions** -Eigenschaft in der [Anwendung](application.md) Entität. Lässt keine Nullwerte zu.            |
|id|Zeichenfolge|Der eindeutige Bezeichner für den Dienstprinzipal. Geerbt von [directoryObject](directoryobject.md). Schlüssel. Lässt keine Nullwerte zu. Schreibgeschützt.|
|passwordCredentials|[PasswordCredential](passwordcredential.md) -Auflistung|Die Auflistung von Anmeldeinformationen den Dienstprinzipal zugeordnet. Lässt keine Nullwerte zu. |
|preferredTokenSigningKeyThumbprint|Zeichenfolge|Nur für interne Zwecke vorbehalten. Schreiben oder verlassen sich andernfalls auf diese Eigenschaft nicht. Kann in zukünftigen Versionen entfernt werden. |
|publisherName|Zeichenfolge|Der Anzeigename des Mandanten in dem verbundenen Anwendung angegeben wird.|
|replyUrls|Collection von Objekten des Typs „String“|Die URLs, dass Benutzertoken, um für die Anmeldung mit der zugeordneten Anwendung oder die Umleitung URIs, dass OAuth 2.0 Autorisierungscodes gesendet werden und Zugriffstoken werden für die zugewiesene Anwendung an. Lässt keine Nullwerte zu. |
|samlMetadataUrl|Zeichenfolge| |
|servicePrincipalNames|Collection von Objekten des Typs „String“|Die URIs, mit denen die zugewiesene Anwendung identifiziert. Weitere Informationen finden Sie unter [Application Objects und Service Principal-Objekte](https://msdn.microsoft.com/library/azure/dn132633.aspx). Der **any** -Operator ist für Filterausdrücke auf mehrwertige Eigenschaften erforderlich.  Lässt keine Nullwerte zu. |
|-Tags hinzugefügtes Markup|Zeichenfolgenauflistung| Lässt keine Nullwerte zu. |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ |Beschreibung|
|:---------------|:--------|:----------|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|Prinzipale (Benutzer, Gruppen und Dienstprinzipale), die diese Dienstprinzipal zugewiesen sind. Schreibgeschützt.|
|appRoleAssignments|[AppRoleAssignment](approleassignment.md) -Auflistung|Anwendungen, denen der Dienstprinzipal zugewiesen ist. Schreibgeschützt. Lässt Nullwerte zu.|
|createdObjects|[directoryObject](directoryobject.md)-Sammlung|Verzeichnis Objekte, die von diesem Dienstprinzipal erstellt. Schreibgeschützt. Lässt Nullwerte zu.|
|memberOf|[directoryObject](directoryobject.md)-Sammlung|Rollen, denen diese Dienstprinzipal ein Mitglied ist. HTTP-Methoden: GET schreibgeschützt. Lässt Nullwerte zu.|
|oauth2PermissionGrants|[oAuth2PermissionGrant](oauth2permissiongrant.md) -Auflistung|Benutzer Identitätswechsel gewährt dieser Dienstprinzipal zugeordnet sind. Schreibgeschützt. Lässt Nullwerte zu.|
|ownedObjects|[directoryObject](directoryobject.md)-Sammlung|Directory-Objekte, die diese Dienstprinzipal gehören. Schreibgeschützt. Lässt Nullwerte zu.|
|owners|[directoryObject](directoryobject.md)-Sammlung|Directory-Objekte, die Besitzer des Prinzipals Service sind. Die Besitzer sind eine Reihe von nicht-Administrator-Benutzer, die berechtigt sind, dieses Objekt zu ändern. Schreibgeschützt. Lässt Nullwerte zu.|
|Richtlinie|Auflistung von [Gruppenrichtlinien](policy.md)|Die Richtlinien, diese Dienstprinzipal zugewiesen sind.|

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von servicePrincipal](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |Lesen Sie Eigenschaften und Beziehungen des ServicePrincipal-Objekts.|
|[Liste servicePrincipals](../api/serviceprincipal-list.md) | [ServicePrincipal](serviceprincipal.md) -Auflistung | Abrufen einer Liste von ServicePrincipal-Objekten. |
|[Erstellen von appRoleAssignment](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| Erstellen Sie eine neue AppRoleAssignment, durch die Veröffentlichung auf der AppRoleAssignments-Auflistung.|
|[Liste appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |[AppRoleAssignment](approleassignment.md) -Auflistung| Rufen Sie eine Auflistung der AppRoleAssignment-Objekts.|
|[List createdObjects](../api/serviceprincipal-list-createdobjects.md) |[directoryObject](directoryobject.md) collection| Rufen Sie eine Auflistung der CreatedObject-Objekts.|
|[memberOf auflisten](../api/serviceprincipal-list-memberof.md) |[directoryObject](directoryobject.md)-Sammlung| Rufen Sie die Gruppen, die dieser Dienst Prinzipal ein direktes Mitglied in der Navigationseigenschaft Mitglied ist.|
|[Transitive Mitglied Liste](../api/serviceprincipal-list-transitivememberof.md) |[directoryObject](directoryobject.md)-Sammlung| Auflisten der Gruppen, denen diese Dienstprinzipal ein Mitglied ist. Dieser Vorgang ist transitiv und enthält die Gruppen, denen dieser Dienst principal geschachtelte Mitglied ist. |
|[Zugewiesen-Listenrichtlinien](../api/policy-list-assigned.md)| Auflistung von [Gruppenrichtlinien](policy.md)| Rufen Sie alle Richtlinien, die auf dieses Objekt zugewiesen.|
|[Liste oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |[oAuth2PermissionGrant](oauth2permissiongrant.md) -Auflistung| Rufen Sie eine Auflistung der oAuth2PermissionGrant-Objekts.|
|[List ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |[directoryObject](directoryobject.md) collection| Rufen Sie eine Auflistung der OwnedObject-Objekts.|
|[Add owner](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| Erstellen Sie einen neuen Besitzer durch die Veröffentlichung auf der Besitzer-Auflistung.|
|[Besitzer auflisten](../api/serviceprincipal-list-owners.md) |[directoryObject](directoryobject.md)-Sammlung| Rufen Sie einen Besitzer Auflistung-Objekts.|
|[Update](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |ServicePrincipal-Objekt zu aktualisieren. |
|[Delete](../api/serviceprincipal-delete.md) | Keine |ServicePrincipal-Objekt zu löschen. |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|Zeichenfolgenauflistung||
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|Zeichenfolgenauflistung||
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|Zeichenfolgenauflistung||
|[delta](../api/serviceprincipal-delta.md)|ServicePrincipal-Auflistung| Möchten Sie inkrementelle Änderungen für Dienstprinzipale erhalten. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
