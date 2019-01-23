---
title: Ressourcentyp managedDeviceCleanupSettings
description: Definieren Sie die Regel aus, wenn der Administrator die Geräte bereinigt werden möchte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4bf756072dcc3cd13bda2fda59b8688b63f3cd43
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424567"
---
# <a name="manageddevicecleanupsettings-resource-type"></a>Ressourcentyp managedDeviceCleanupSettings

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Definieren Sie die Regel aus, wenn der Administrator die Geräte bereinigt werden möchte.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|deviceInactivityBeforeRetirementInDays|Zeichenfolge|Anzahl der Tage, wenn das Gerät nicht Intune kontaktiert hat.|

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




