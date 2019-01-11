---
title: " Ressourcentyp controlScore"
description: Diese Ressource enthält einen Mandanten Score und eine Beschreibung für ein einzelnes Steuerelement.
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891469"
---
#  <a name="controlscore-resource-type"></a>Ressourcentyp controlScore

Diese Ressource enthält einen Mandanten Score und eine Beschreibung für ein einzelnes Steuerelement.

|Name |Typ |Beschreibung |
|:--|:--|:--|
|   Steuerelementname |   Zeichenfolge  |   Eindeutiger Name des Steuerelements |
|   score   |   Gleitkommawert mit doppelter Genauigkeit  |  Mandanten erreicht Score für das Steuerelement (Dies hängt Tag je nach Mandant Vorgänge auf das Steuerelement). |
|   controlCategory |   Zeichenfolge  |  Steuerelement-Aktionskategorie (Identität, Daten, Gerät, Apps, Infrastruktur). |
|   description |   Zeichenfolge  |  Beschreibung des Steuerelements. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.controlScore"
}-->

```json
{
  "controlName": "String",
  "score": "String",
  "controlCategory": "String",
  "description": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "controlScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
