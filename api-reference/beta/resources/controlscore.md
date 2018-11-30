---
title: " Ressourcentyp controlScore"
description: Diese Ressource enthält einen Mandanten Score und eine Beschreibung für ein einzelnes Steuerelement.
ms.openlocfilehash: 67059c1a7382416411709f02c609c90b20a673b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059474"
---
#  <a name="controlscore-resource-type"></a>Ressourcentyp controlScore

Diese Ressource enthält einen Mandanten Score und eine Beschreibung für ein einzelnes Steuerelement.

|Name |Typ |Beschreibung |
|:--|:--|:--|
|   Steuerelementname |   String  |   Eindeutiger Name des Steuerelements |
|   score   |   Gleitkommawert mit doppelter Genauigkeit  |  Mandanten erreicht Score für das Steuerelement (Dies hängt Tag je nach Mandant Vorgänge auf das Steuerelement). |
|   controlCategory |   String  |  Steuerelement-Aktionskategorie (Identität, Daten, Gerät, Apps, Infrastruktur). |
|   description |   String  |  Beschreibung des Steuerelements. |

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
