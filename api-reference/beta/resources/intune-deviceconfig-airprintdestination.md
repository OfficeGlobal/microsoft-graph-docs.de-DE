---
title: airPrintDestination-Ressourcentyp
description: Stellt ein Druckziel dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f09301bd791b5fd8b3fa430b50f7cdf58de43944
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167333"
---
# <a name="airprintdestination-resource-type"></a>airPrintDestination-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt ein Druckziel dar.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ipAddress|Zeichenfolge|Die IP-Adresse des Druckziels.|
|resourcePath|Zeichenfolge|Der dem Drucker zugeordnete Ressourcenpfad. Dies entspricht dem RP-Parameter des Bonjour-Eintrags _ipps. TCP. Beispiel: Printers/Canon_MG5300_series, Printers/Xerox_Phaser_7600, IPP/Print, Epson_IPP_Printer.|
|port|Int32|Der Überwachungs-Port des Druckziels. Wenn dieser Schlüssel nicht angegeben ist, verwendet der standardmäßige Port. Verfügbar in iOS 11,0 und höher.|
|forceTls|Boolescher Wert|Wenn true-druckverbindungs Verbindungen durch Transport Layer Security (TLS) gesichert werden. Der Standardwert ist false. Verfügbar in iOS 11,0 und höher.|

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




