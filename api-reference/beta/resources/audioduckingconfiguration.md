---
title: Ressourcentyp audioDuckingConfiguration
description: Parameter für Vermeiden von anderen Quellen (können in und aus anderen Quellen).
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4132946573342976bb1f20c593454a8e18030d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916873"
---
# <a name="audioduckingconfiguration-resource-type"></a>Ressourcentyp audioDuckingConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Parameter für Vermeiden von anderen Quellen (können in und aus anderen Quellen).

## <a name="properties"></a>Eigenschaften

| Eigenschaft      | Typ     | Beschreibung                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| lowerLevel    | Int64    | Das Volumen der Quellen in Prozent, wenn Sie die Quellen sind ducked wird.             |
| rampActive    | Int64    | Die Zeitdauer (in Millisekunden) für ducked Datenquellen "Verblassen" dauert. |
| rampInactive  | Int64    | Die Zeitdauer (in Millisekunden) für ducked Datenquellen für eine "einblenden" dauert.  |
| upperLevel    | Int64    | Das Volumen der Quellen in Prozent, wenn Sie die Quellen sind nicht ducked wird.         |

> **Hinweis:** Lernen Dauer kann nicht mehr als 5000 Millisekunden sein.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioDuckingConfiguration"
}-->
```json
{
  "lowerLevel": 20,
  "rampActive": 1000,
  "rampInactive": 1000,
  "upperLevel": 100
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
