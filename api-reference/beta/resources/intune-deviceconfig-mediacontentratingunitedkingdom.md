---
title: mediaContentRatingUnitedKingdom-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e4ab6731bc486918815efe0d3f4c7f6f2638329d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953301"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a>mediaContentRatingUnitedKingdom-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|movieRating|[ratingUnitedKingdomMoviesType](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|Bewertung für Großbritannien ausgewählten Filme. Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.|
|tvRating|[ratingUnitedKingdomTelevisionType](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|TV-Bewertung für Großbritannien ausgewählt. Mögliche Werte sind: `allAllowed`, `allBlocked` und `caution`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```





