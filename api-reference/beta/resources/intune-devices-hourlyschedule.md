---
title: hourlySchedule-Ressourcentyp
description: Stündlicher Ausführungszeitplan für ein wiederkehrendes Geräte Verwaltungsskript.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb3eacf4e17ed1137ce78d21112c394a45423c6b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173416"
---
# <a name="hourlyschedule-resource-type"></a>hourlySchedule-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stündlicher Ausführungszeitplan für ein wiederkehrendes Geräte Verwaltungsskript.


Erbt von [runSchedule](../resources/intune-devices-runschedule.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|Intervall|Int32|Intervall in Stunden|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hourlySchedule",
  "interval": 1024
}
```




