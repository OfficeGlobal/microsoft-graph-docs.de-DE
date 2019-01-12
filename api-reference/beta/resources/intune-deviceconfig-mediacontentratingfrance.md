---
title: mediaContentRatingFrance-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7aa3c16df6b32f5c5c50f53959aaccc767b39bbd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928143"
---
# <a name="mediacontentratingfrance-resource-type"></a>mediaContentRatingFrance-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|movieRating|[ratingFranceMoviesType](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|Bewertung für Frankreich ausgewählten Filme. Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.|
|tvRating|[ratingFranceTelevisionType](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|TV-Bewertung für Frankreich ausgewählt. Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```





