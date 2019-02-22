---
title: win32LobAppProductCodeDetection-Ressourcentyp
description: Enthält Produktcode-und Versionseigenschaften zum Auffinden einer Win32-App
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 854d54b034b0e2e0dc0e7ce8e7f73466f37dd263
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173234"
---
# <a name="win32lobappproductcodedetection-resource-type"></a>win32LobAppProductCodeDetection-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Produktcode-und Versionseigenschaften zum Auffinden einer Win32-App


Erbt von [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|productCode|Zeichenfolge|Der Produktcode der Win32-Branchen-app.|
|productVersionOperator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|Der Operator, der die Produktversion ermittelt. Mögliche Werte sind: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan` und `lessThanOrEqual`.|
|productVersion|Zeichenfolge|Die Produktversion der Win32-Branchen-app.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeDetection",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```




