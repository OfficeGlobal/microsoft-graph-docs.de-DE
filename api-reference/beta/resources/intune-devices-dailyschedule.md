---
title: dailySchedule-Ressourcentyp
description: Täglicher Ausführungszeitplan für ein wiederkehrendes Geräte Verwaltungsskript.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 310d9a4dbd995dfc162591547a40ace8c596f54b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152661"
---
# <a name="dailyschedule-resource-type"></a>dailySchedule-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Täglicher Ausführungszeitplan für ein wiederkehrendes Geräte Verwaltungsskript.


Erbt von [runSchedule](../resources/intune-devices-runschedule.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|Intervall|Int32|Intervall in Tagen|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dailySchedule",
  "interval": 1024
}
```




