---
title: managedAppDiagnosticStatus-Ressourcentyp
description: Stellt den Diagnosestatus dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf91e1a86955612aa590bee68057e1a7adb2d823
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169006"
---
# <a name="managedappdiagnosticstatus-resource-type"></a>managedAppDiagnosticStatus-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt den Diagnosestatus dar.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|validationName|Zeichenfolge|Der leicht zu prüfende Name|
|state|Zeichenfolge|Der Status des Vorgangs|
|mitigationInstruction|Zeichenfolge|Anweisungen zum Umgehen einer fehlgeschlagenen Validierung|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```




