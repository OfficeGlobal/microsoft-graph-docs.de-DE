---
title: win32LobAppRegistryDetection-Ressourcentyp
description: Enthält Registrierungseigenschaften zum Auffinden einer Win32-App
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 076251ea185359127c3dad3610ec944f7cdb3178
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169545"
---
# <a name="win32lobappregistrydetection-resource-type"></a>win32LobAppRegistryDetection-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Registrierungseigenschaften zum Auffinden einer Win32-App


Erbt von [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|check32BitOn64System|Boolescher Wert|Ein Wert, der angibt, ob dieser Registrierungspfad zum Überprüfen der 32-Bit-App auf dem 64-Bit-System dient.|
|keyPath|Zeichenfolge|Registrierungsschlüsselpfad zum Aufspüren der Win32-Branchen-App|
|valueName|Zeichenfolge|Der Name des Registrierungswerts|
|detectiontype|[win32LobAppRegistryDetectionType](../resources/intune-apps-win32lobappregistrydetectiontype.md)|Der Erkennungstyp der Registrierungsdaten. Mögliche Werte sind: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer` und `version`.|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|Der Operator für die Erkennung von Registrierungsdaten. Mögliche Werte sind: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan` und `lessThanOrEqual`.|
|Erkennungs-Value|Zeichenfolge|Der Registrierungs Erkennungswert|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryDetection",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```




