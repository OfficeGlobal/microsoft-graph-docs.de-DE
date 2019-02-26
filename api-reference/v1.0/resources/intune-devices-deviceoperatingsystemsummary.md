---
title: deviceOperatingSystemSummary-Ressourcentyp
description: Betriebssystemzusammenfassung für das Gerät
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53c806e250d6b201e6dfe49d90685c4144913182
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250404"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a>deviceOperatingSystemSummary-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Betriebssystem des Geräts – Zusammenfassung.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|androidCount|Int32|Anzahl der Android-Geräte.|
|iosCount|Int32|Anzahl der iOS-Geräte.|
|macOSCount|Int32|Anzahl der Mac OS X-Geräte.|
|windowsMobileCount|Int32|Anzahl der Windows Mobile-Geräte.|
|windowsCount|Int32|Anzahl der Windows-Geräte.|
|unknownCount|Int32|Anzahl von unbekannten Geräten.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```



