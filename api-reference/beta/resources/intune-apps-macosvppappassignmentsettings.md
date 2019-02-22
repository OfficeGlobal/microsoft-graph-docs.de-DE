---
title: macOsVppAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen Mac VPP-APP zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 102869101b577eadb40eb4a3146c45e422d9c24a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150981"
---
# <a name="macosvppappassignmentsettings-resource-type"></a>macOsVppAppAssignmentSettings-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften zum Zuweisen einer mobilen Mac VPP-APP zu einer Gruppe.


Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|useDeviceLicensing|Boolescher Wert|Gibt an, ob die Gerätelizenzierung verwendet werden soll oder nicht.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignmentSettings",
  "useDeviceLicensing": true
}
```




