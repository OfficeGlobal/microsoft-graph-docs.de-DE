---
title: Ressourcentyp audioSourceLevel
description: Konfiguration für andere Datenquellen.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c91a4c57b283f7669b2be22bba5de5d958b437ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528375"
---
# <a name="audiosourcelevel-resource-type"></a>Ressourcentyp audioSourceLevel

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Konfiguration für andere Datenquellen.

## <a name="properties"></a>Eigenschaften

| Eigenschaft               | Typ    | Beschreibung                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| duckOthers             | Boolescher Wert | Dieser Quelle zu anderen Quellen, während es aktiv Wildenten ermöglicht. Wenn auf true festgelegt ist, vermeiden Ebene festgelegt ist festgelegt werden soll.|
| Ebene                  | Int64   | Ebene der Quelle vermeiden, wenn `duckOthers` auf festgelegt ist `true`.                                     |
| Teilnehmer            | String  | Die Teilnehmer Audiostream von Quelle.                                                                |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioSourceLevel"
}-->
```json
{
  "duckOthers": true,
  "level": 100,
  "participant": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audiosourcelevel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
