---
title: Ressourcentyp preAuthorizedApplication
description: Stellt eine Anwendung und die angeforderten Berechtigungen für implizite Zustimmung dar. Erfordert ein Administrator Zustimmung an die Anwendung bereitgestellt haben. PreAuthorizedApplications erfordern keinen den Benutzer, die angeforderten Berechtigungen zuzustimmen. In PreAuthorizedApplications aufgelisteten Berechtigungen erfordern keine Zustimmung des Benutzers. Keine weiteren angeforderten Berechtigungen nicht in PreAuthorizedApplications aufgeführten erfordern jedoch Zustimmung des Benutzers.
localization_priority: Normal
ms.openlocfilehash: 22945589341066f4609d47773cb04426774648fd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524548"
---
# <a name="preauthorizedapplication-resource-type"></a>Ressourcentyp preAuthorizedApplication

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Anwendung und die angeforderten Berechtigungen für implizite Zustimmung dar. Erfordert ein Administrator Zustimmung an die Anwendung bereitgestellt haben. PreAuthorizedApplications erfordern keinen den Benutzer, die angeforderten Berechtigungen zuzustimmen. In PreAuthorizedApplications aufgelisteten Berechtigungen erfordern keine Zustimmung des Benutzers. Keine weiteren angeforderten Berechtigungen nicht in PreAuthorizedApplications aufgeführten erfordern jedoch Zustimmung des Benutzers.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|appId|Zeichenfolge| Der eindeutige Bezeichner für die Anwendung. |
|permissionIds|Zeichenfolgenauflistung| Der eindeutige Bezeichner für die [PublishedPermissionScope](permissionscope.md) oder [AppRole](approle.md) die Anwendung erfordert. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "permissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/preauthorizedapplication.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
