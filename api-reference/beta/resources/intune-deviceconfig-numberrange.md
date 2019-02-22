---
title: numberRange-Ressourcentyp
description: Nummernkreis Definition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 711206a256e17d6e10c7c54cf8a3dda4868db031
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166787"
---
# <a name="numberrange-resource-type"></a>numberRange-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Nummernkreis Definition.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|lowerNumber|Int32|Niedrigere Zahl.|
|upperNumber|Int32|Obere Zahl.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```




