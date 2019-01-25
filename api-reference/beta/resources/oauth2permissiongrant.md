---
title: Ressourcentyp oAuth2PermissionGrant
description: Stellt die OAuth 2.0-Bereiche (delegierten Berechtigungen) zu einer Anwendung (dargestellt durch ein Dienstprinzipal) erteilt wurden im Rahmen des Prozesses Zustimmung Benutzer oder Administrator an.
localization_priority: Normal
ms.openlocfilehash: ea6486aedca4c3fcf73e59a5652ccf517fb01ddc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516924"
---
# <a name="oauth2permissiongrant-resource-type"></a>Ressourcentyp oAuth2PermissionGrant

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|clientId|String| Die Id des Prinzipals Dienst gewährt Ihr Einverständnis der Benutzer Identitätswechsel für den Zugriff auf die Ressource (dargestellt durch die ResourceId-Eigenschaft). |
|consentType|String| Gibt an, ob Zustimmung vom Administrator (im Namen der Organisation) oder von einer Person zur Verfügung gestellt wurde. Mögliche Werte sind „AllPrincipals“ oder „Principal“. |
|ExpiryTime|DateTimeOffset| Derzeit ist der Ablauf Time-Wert ignoriert. |
|id|Zeichenfolge| Eindeutiger Bezeichner Schreibgeschützt.|
|principalId|String| Wenn ConsentType *AllPrincipals* ist dieser Wert ist null, und die Zustimmung gilt für alle Benutzer in der Organisation. Wenn ConsentType *Prinzipal*ist, gibt diese Eigenschaft die Id des Benutzers, der Zustimmung erteilt und gilt nur für diesen Benutzer an. |
|resourceId|Zeichenfolge| Gibt die Id des Prinzipals Service Resource, der Zugriff gewährt wurde. |
|Bereich|String| Gibt den Wert des Anspruchs [Bereich](/graph/permissions-reference) , der die Ressource Anwendung erwarten im Zugriffstoken OAuth 2.0 an. Beispielsweise *User.Read* |
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
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permissiongrant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
