---
title: Ressourcentyp audioSourceLevel
description: Konfiguration für andere Datenquellen.
ms.openlocfilehash: 527cb7e104817dc19287195d625bfc5f88c14e1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065449"
---
# <a name="audiosourcelevel-resource-type"></a>Ressourcentyp audioSourceLevel

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Konfiguration für andere Datenquellen.

## <a name="properties"></a>Eigenschaften

| Eigenschaft               | Typ    | Beschreibung                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| duckOthers             | Boolesch | Dieser Quelle zu anderen Quellen, während es aktiv Wildenten ermöglicht. Wenn auf true festgelegt ist, vermeiden Ebene festgelegt ist festgelegt werden soll.|
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
<!-- {
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
