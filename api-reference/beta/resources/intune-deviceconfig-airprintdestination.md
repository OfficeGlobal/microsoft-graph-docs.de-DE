---
title: Ressourcentyp airPrintDestination
description: Stellt ein AirPrint Ziel.
ms.openlocfilehash: a1f30f5c71a8ee79bb537ad4ae1f20ce8a05d184
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060469"
---
# <a name="airprintdestination-resource-type"></a>Ressourcentyp airPrintDestination

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt ein AirPrint Ziel.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ipAddress|Zeichenfolge|Die IP-Adresse des Ziels AirPrint.|
|Http://|String|Der Pfad der Ressource mit dem Drucker verknüpft ist. Dies entspricht dem Rp-Parameter, der die _ipps.tcp Bonjour Datensatz. Beispiel: Drucker/Canon_MG5300_series, Drucker/Xerox_Phaser_7600, Ipp/Epson_IPP_Printer drucken.|
|port|Int32|Der Überwachungsport des Ziels AirPrint. Wenn dieser Schlüssel nicht angegeben ist, wird AirPrint den Standardport verwenden. In iOS 11.0 und höher verfügbar.|
|forceTls|Boolesch|Wenn true AirPrint Verbindungen von Transport Layer Security (TLS) gesichert werden. Standard ist false. In iOS 11.0 und höher verfügbar.|

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





