---
title: Ressourcentyp configurationManagerClientHealthState
description: Konfigurations-Manager-Client-Zustand
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55ba2b24df0d1d4c278f4785a310237c9c32cd9b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425827"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a>Ressourcentyp configurationManagerClientHealthState

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Konfigurations-Manager-Client-Zustand

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|state|[configurationManagerClientState](../resources/intune-devices-configurationmanagerclientstate.md)|Aktuelle Configuration Manager-Client-Zustand. Mögliche Werte sind: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed` und `communicationError`.|
|errorCode|Int32|Der Fehlercode für ausgefallenen Zustand.|
|lastSyncDateTime|DateTimeOffset|Zeigen Sie DateTime fo letzte Synchronisierung mit Configuration Manager-Management.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
  "state": "String",
  "errorCode": 1024,
  "lastSyncDateTime": "String (timestamp)"
}
```




