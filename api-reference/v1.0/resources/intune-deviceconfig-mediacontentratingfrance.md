---
title: mediaContentRatingFrance-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 0981a73fdc1e8468d9e8ab8590387dfa357a39c9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361642"
---
# <a name="mediacontentratingfrance-resource-type"></a>mediaContentRatingFrance-Ressourcentyp

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



