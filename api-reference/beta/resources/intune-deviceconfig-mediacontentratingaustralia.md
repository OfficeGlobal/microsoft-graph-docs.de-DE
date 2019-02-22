---
title: mediaContentRatingAustralia-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae1cb934af017c751ae2bcf05cd992668a452ed6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166766"
---
# <a name="mediacontentratingaustralia-resource-type"></a>mediaContentRatingAustralia-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Noch nicht dokumentiert

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|movieRating|[ratingAustraliaMoviesType](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|Film Bewertung für Australien ausgewählt. Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15` und `agesAbove18`.|
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




