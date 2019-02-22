---
title: managedDeviceModelsAndManufacturers-Ressourcentyp
description: Modelliert und fertigt meatadata für verwaltete Geräte im Konto
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfd8f068305bdae86a0acc9ef5f9113bb0d1c579
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148300"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a>managedDeviceModelsAndManufacturers-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Modelliert und fertigt meatadata für verwaltete Geräte im Konto

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|deviceModels|String collection|Liste der Modelle für verwaltete Geräte im Konto|
|deviceManufacturers|String collection|Liste der Hersteller für verwaltete Geräte im Konto|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```




