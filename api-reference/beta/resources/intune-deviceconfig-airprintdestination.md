---
title: Ressourcentyp airPrintDestination
description: Stellt ein AirPrint Ziel.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f56578427427d45a69c4c64fe9fde3cf31f8fd9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422495"
---
# <a name="airprintdestination-resource-type"></a>Ressourcentyp airPrintDestination

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Stellt ein AirPrint Ziel.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ipAddress|Zeichenfolge|Die IP-Adresse des Ziels AirPrint.|
|Http://|Zeichenfolge|Der Pfad der Ressource mit dem Drucker verknüpft ist. Dies entspricht dem Rp-Parameter, der die _ipps.tcp Bonjour Datensatz. Beispiel: Drucker/Canon_MG5300_series, Drucker/Xerox_Phaser_7600, Ipp/Epson_IPP_Printer drucken.|
|port|Int32|Der Überwachungsport des Ziels AirPrint. Wenn dieser Schlüssel nicht angegeben ist, wird AirPrint den Standardport verwenden. In iOS 11.0 und höher verfügbar.|
|forceTls|Boolean|Wenn true AirPrint Verbindungen von Transport Layer Security (TLS) gesichert werden. Standard ist false. In iOS 11.0 und höher verfügbar.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.airPrintDestination"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.airPrintDestination",
  "ipAddress": "String",
  "resourcePath": "String",
  "port": 1024,
  "forceTls": true
}
```




