---
title: macOSLobChildApp-Ressourcentyp
description: Enthält Eigenschaften der MacOS-Branchen-app in einem Bundle-Paket
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4bf8a8715bb681d1737a2fb1b39e5bac61fb9d7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146998"
---
# <a name="macoslobchildapp-resource-type"></a>macOSLobChildApp-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften der MacOS-Branchen-app in einem Bundle-Paket

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|bundleId|Zeichenfolge|Identitätsname|
|buildNumber|Zeichenfolge|Die Buildnummer der MacOS-app.|
|versionNumber|Zeichenfolge|Die Versionsnummer der MacOS-app.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```




