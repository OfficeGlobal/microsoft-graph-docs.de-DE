---
title: windowsKioskLocalGroup-Ressourcentyp
description: Die Klasse, die zum Identifizieren einer lokalen Gruppe für die Kiosk Konfiguration verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3479226d770c7030fefed1a7f2f65a02808479d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169524"
---
# <a name="windowskiosklocalgroup-resource-type"></a>windowsKioskLocalGroup-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Klasse, die zum Identifizieren einer lokalen Gruppe für die Kiosk Konfiguration verwendet wird.


Erbt von [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|groupName|Zeichenfolge|Der Name der lokalen Gruppe, die für diese Kiosk Konfiguration gesperrt wird.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalGroup",
  "groupName": "String"
}
```




