---
title: Ressourcentyp managedDeviceModelsAndManufacturers
description: Modelle und Hersteller Meatadata für verwaltete Geräte im Konto
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 86d9f9dd0642abab73f6b750b997c75851f6be02
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875621"
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





