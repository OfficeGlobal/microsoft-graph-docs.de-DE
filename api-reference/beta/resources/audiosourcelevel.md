---
title: Ressourcentyp audioSourceLevel
description: Konfiguration für andere Datenquellen.
author: VinodRavichandran
ms.openlocfilehash: 5d5abe7eba03891427b30ba1c8f63b15b3707e46
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380240"
---
# <a name="audiosourcelevel-resource-type"></a>Ressourcentyp audioSourceLevel

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Konfiguration für andere Datenquellen.

## <a name="properties"></a>Eigenschaften

| Eigenschaft               | Typ    | Beschreibung                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| duckOthers             | Boolescher Wert | Dieser Quelle zu anderen Quellen, während es aktiv Wildenten ermöglicht. Wenn auf true festgelegt ist, vermeiden Ebene festgelegt ist festgelegt werden soll.|
| Ebene                  | Int64   | Ebene der Quelle vermeiden, wenn `duckOthers` auf festgelegt ist `true`.                                     |
| Teilnehmer            | Zeichenfolge  | Die Teilnehmer Audiostream von Quelle.                                                                |

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
<!-- {
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
