---
title: microsoftStoreForBusinessAppAssignmentSettings-Ressourcentyp
description: Enthält die Eigenschaften, die verwendet werden, um eine mobile Microsoft Store für Unternehmen-App einer Gruppe zuzuweisen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1aed45ba54abdcb25f5436beeb2a03f53b9dbae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261103"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a>microsoftStoreForBusinessAppAssignmentSettings-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält die Eigenschaften, die verwendet werden, um eine mobile Microsoft Store für Unternehmen-App einer Gruppe zuzuweisen.


Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|useDeviceContext|Boolescher Wert|Gibt an, ob der Geräte-Ausführungskontext für mobile Microsoft Store für Unternehmen-Apps verwendet werden soll oder nicht.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```



