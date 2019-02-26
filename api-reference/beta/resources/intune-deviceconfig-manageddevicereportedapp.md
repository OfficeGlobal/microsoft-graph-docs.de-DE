---
title: managedDeviceReportedApp-Ressourcentyp
description: Anwendungsdaten für die Berichterstellung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3e1cd99974259835859cf8a2fc6a9f197c09d4d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166269"
---
# <a name="manageddevicereportedapp-resource-type"></a>managedDeviceReportedApp-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Anwendungsdaten für die Berichterstellung

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|appId|Zeichenfolge|Anwendungs- oder Paket-ID der Anwendung|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceReportedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceReportedApp",
  "appId": "String"
}
```




