---
title: configurationManagerClientEnabledFeatures-Ressourcentyp
description: Im Konfigurations-Manager-Client aktivierte Features
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7975130bb047e097ea0d52a4ce770fb35e4efa32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425904"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>configurationManagerClientEnabledFeatures-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Im Konfigurations-Manager-Client aktivierte Features

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|inventory|Boolean|Gibt an, ob der Bestand von Intune verwaltet wird|
|modernApps|Boolean|Gibt an, ob die moderne Anwendung von Intune verwaltet wird|
|resourceAccess|Boolean|Gibt an, ob der Zugriff auf Ressourcen von Intune verwaltet wird|
|deviceConfiguration|Boolean|Gibt an, ob die Gerätekonfiguration von Intune verwaltet wird|
|compliancePolicy|Boolean|Gibt an, ob Compliance-Richtlinie von Intune verwaltet wird|
|windowsUpdateForBusiness|Boolean|Gibt an, ob Windows Update for Business von Intune verwaltet wird|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```




