---
title: vppLicensingType-Ressourcentyp
description: Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f09ca9a8f891b90563ebad2cff74775f4c6fb7c2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168397"
---
# <a name="vpplicensingtype-resource-type"></a>vppLicensingType-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|supportUserLicensing|Boolescher Wert|Gibt an, ob das Programm den Benutzerlizenzierungstyp unterstützt.|
|supportDeviceLicensing|Boolescher Wert|Gibt an, ob das Programm den Gerätelizenzierungstyp unterstützt.|
|supportsUserLicensing|Boolescher Wert|Gibt an, ob das Programm den Benutzerlizenzierungstyp unterstützt.|
|supportsDeviceLicensing|Boolescher Wert|Gibt an, ob das Programm den Gerätelizenzierungstyp unterstützt.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```




