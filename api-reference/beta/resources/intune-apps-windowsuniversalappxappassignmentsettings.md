---
title: windowsUniversalAppXAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften, die beim Zuweisen einer mobilen Windows Mobile-AppX-APP zu einer Gruppe verwendet werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58e0c656464d962d1a16a7c4651c4379876bf6ae
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153732"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a>windowsUniversalAppXAppAssignmentSettings-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften, die beim Zuweisen einer mobilen Windows Mobile-AppX-APP zu einer Gruppe verwendet werden.


Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|useDeviceContext|Boolescher Wert|Gibt an, ob der Geräte Ausführungskontext für die Mobile Windows Universal AppX-App verwendet werden soll.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUniversalAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```




