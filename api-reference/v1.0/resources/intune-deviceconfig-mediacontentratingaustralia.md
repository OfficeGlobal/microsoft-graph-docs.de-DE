---
title: mediaContentRatingAustralia-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5f3f12cc233c1accfad05ccec92d412c75426d1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952846"
---
# <a name="mediacontentratingaustralia-resource-type"></a>mediaContentRatingAustralia-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|movieRating|[ratingAustraliaMoviesType](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|Bewertung für Australien ausgewählten Filme. Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15` und `agesAbove18`.|
|tvRating|[ratingAustraliaTelevisionType](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|TV-Bewertung für Australien ausgewählt. Mögliche Werte: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



