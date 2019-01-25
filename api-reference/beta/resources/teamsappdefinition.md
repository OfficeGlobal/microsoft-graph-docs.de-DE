---
title: Ressourcentyp teamsAppDefinition
description: Die Details einer Version von einer TeamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 94e2c790f8bf4623e56ca76bde164b718ee6fa38
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509980"
---
# <a name="teamsappdefinition-resource-type"></a>Ressourcentyp teamsAppDefinition

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die Details einer Version von einer [TeamsApp](teamsapp.md).

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ     | Beschreibung |
|:------------------- |:-------- |:----------- |
| id                  | string   | Eine eindeutige Id (nicht die Teams Appid). |
| teamsAppId          | string   | Die Id von Teams App-Manifest. |
| displayName         | string   | Der Name der app bereitgestellt von der app-Entwickler. |
| Version             | string   | Die Versionsnummer der Anwendung. |

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0",
}
```

# <a name="see-also"></a>Siehe auch

- [teamsApp](teamsapp.md)
- [teamsAppInstallation](teamsappinstallation.md)
- [teamsTab](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappdefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

