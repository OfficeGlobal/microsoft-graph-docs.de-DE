---
title: vppLicensingType-Ressourcentyp
description: Enthält Eigenschaften für den iOS-Volume-Purchased Programm (Vpp)-Lizenzierungstyp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 42bb678077781309b9e06c339112537bc2e48bde
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399675"
---
# <a name="vpplicensingtype-resource-type"></a>vppLicensingType-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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




