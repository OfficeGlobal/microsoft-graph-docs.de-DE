---
title: API-Ressourcentyp
description: Gibt die Einstellungen für eine-API-Webanwendung.
ms.openlocfilehash: b5b07ccb5a66027f9eb755754842f6e2e2ae708e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060464"
---
# <a name="api-resource-type"></a>API-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Gibt die Einstellungen für eine-API-Webanwendung.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|requestedAccessTokenVersion|Int32| Gibt die Version der akzeptierten Access token für die aktuelle API-Ressource. Mögliche Werte sind 1 oder 2.  |
|oauth2PermissionScopes|[PermissionScope](permissionscope.md) -Auflistung| Die Auflistung von OAuth 2.0-berechtigungsbereiche, die im Web-API (Ressource) Anwendung Clientanwendungen verfügbar macht. Diese berechtigungsbereiche können während der Zustimmung Clientanwendungen gewährt werden. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.api"
}-->

```json
{
  "requestedAccessTokenVersion": 1,
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->