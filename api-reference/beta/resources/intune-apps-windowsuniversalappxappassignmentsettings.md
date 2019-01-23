---
title: Ressourcentyp windowsUniversalAppXAppAssignmentSettings
description: Enthält Eigenschaften verwendet, wenn eine universelle AppX Windows mobile app zu einer Gruppe zuweisen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27755a483be44584aeb82166f56e825df79f8eaa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400718"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a>Ressourcentyp windowsUniversalAppXAppAssignmentSettings

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Enthält Eigenschaften verwendet, wenn eine universelle AppX Windows mobile app zu einer Gruppe zuweisen.


Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|useDeviceContext|Boolescher Wert|Ob Ausführungskontexts Gerät für universelle AppX Windows mobile app verwenden.|

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




