---
title: Ressourcentyp managedDeviceModelsAndManufacturers
description: Modelle und Hersteller Meatadata für verwaltete Geräte im Konto
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8a1769f82153fd8184807877c484a4dc31ebda1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927527"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a>Ressourcentyp managedDeviceModelsAndManufacturers

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Modelle und Hersteller Meatadata für verwaltete Geräte im Konto
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|deviceModels|Collection von Objekten des Typs „String“|Liste der Modelle für verwaltete Geräte im Konto|
|deviceManufacturers|Collection von Objekten des Typs „String“|Liste der Hersteller für verwalteten Geräten im Konto|

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





