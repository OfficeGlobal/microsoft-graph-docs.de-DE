---
title: managedDeviceCleanupSettings-Ressourcentyp
description: Definieren Sie die Regel, wenn der Administrator möchte, dass die Geräte bereinigt werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76abaf4cb06156881a530d50e3322e649eedde51
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148482"
---
# <a name="manageddevicecleanupsettings-resource-type"></a>managedDeviceCleanupSettings-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Definieren Sie die Regel, wenn der Administrator möchte, dass die Geräte bereinigt werden.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|deviceInactivityBeforeRetirementInDays|Zeichenfolge|Anzahl der Tage, an denen das Gerät InTune nicht kontaktiert hat.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceCleanupSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCleanupSettings",
  "deviceInactivityBeforeRetirementInDays": "String"
}
```




