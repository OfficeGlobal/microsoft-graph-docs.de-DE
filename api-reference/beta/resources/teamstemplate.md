---
title: Ressourcentyp teamsTemplate
description: Beschreibt die TeamsTemplate Entität.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e75b3d8df318b116d5d908a40d4f756d9ee70864
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513046"
---
# <a name="teamstemplate-resource-type"></a>Ressourcentyp teamsTemplate

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine Teamvorlage ist eine Vorlage für ein [Team](../resources/team.md) in Microsoft-Teams erstellen. Eine Vorlage gibt die Struktur, Einstellungen und sogar Inhalte, die bereitgestellt werden soll in ein neues Team mit der Vorlage erstellt. Microsoft bietet eine Reihe von Basis Vorlagen und Kunden können ihre eigenen benutzerdefinierten Vorlagen gespeichert.

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ     | Beschreibung |
|:------------------- |:-------- |:----------- |
| id                  | String   | Eindeutiger Bezeichner der Vorlage. Darf nicht null sein. |

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a>Siehe auch

- Team

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
