---
title: Ressourcentyp oAuth2PermissionGrant
description: Stellt die OAuth 2.0-Bereiche (delegierten Berechtigungen) zu einer Anwendung (dargestellt durch ein Dienstprinzipal) erteilt wurden im Rahmen des Prozesses Zustimmung Benutzer oder Administrator an.
localization_priority: Normal
ms.openlocfilehash: 835e4a2c1a8d19c9c21e706adbf2f10a6a505bb3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884448"
---
# <a name="oauth2permissiongrant-resource-type"></a>Ressourcentyp oAuth2PermissionGrant

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die OAuth 2.0-Bereiche (delegierten Berechtigungen) zu einer Anwendung (dargestellt durch ein Dienstprinzipal) erteilt wurden im Rahmen des Prozesses Zustimmung Benutzer oder Administrator an.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "expiryTime": "String (timestamp)",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string",
  "startTime": "String (timestamp)"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|clientId|Zeichenfolge| Die Id des Prinzipals Dienst gewährt Ihr Einverständnis der Benutzer Identitätswechsel für den Zugriff auf die Ressource (dargestellt durch die ResourceId-Eigenschaft). |
|consentType|Zeichenfolge| Gibt an, ob Zustimmung vom Administrator (im Namen der Organisation) oder von einer Person zur Verfügung gestellt wurde. Die möglichen Werte sind *AllPrincipals* oder *Prinzipal*. |
|expiryTime|DateTimeOffset| Derzeit ist der Ablauf Time-Wert ignoriert. |
|id|Zeichenfolge| Eindeutiger Bezeichner. Schreibgeschützt.|
|principalId|Zeichenfolge| Wenn ConsentType *AllPrincipals* ist dieser Wert ist null, und die Zustimmung gilt für alle Benutzer in der Organisation. Wenn ConsentType *Prinzipal*ist, gibt diese Eigenschaft die Id des Benutzers, der Zustimmung erteilt und gilt nur für diesen Benutzer an. |
|resourceId|Zeichenfolge| Gibt die Id des Prinzipals Service Resource, der Zugriff gewährt wurde. |
|scope|Zeichenfolge| Gibt den Wert des Anspruchs [Bereich](/graph/permissions-reference) , der die Ressource Anwendung erwarten im Zugriffstoken OAuth 2.0 an. Beispielsweise *User.Read* |
|startTime|DateTimeOffset| Derzeit wird der Wert für die Startzeit ignoriert. |

## <a name="relationships"></a>Beziehungen
Keine


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |Lesen Sie Eigenschaften und Beziehungen des oAuth2PermissionGrant-Objekts.|
|[Liste oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) -Auflistung | Abrufen einer Liste von oauth2PermissionGrant-Objekten. |
|[OAuth2PermissionGrant aktualisieren](../api/oauth2permissiongrant-update.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |OAuth2PermissionGrant-Objekt zu aktualisieren. |
|[OAuth2PermissionGrant löschen](../api/oauth2permissiongrant-delete.md) | Keine |OAuth2PermissionGrant-Objekt zu löschen. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
