---
title: Ressourcentyp windowsUpdateState
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 20387d9e1fd9b84853a7bc097dfa08d128809358
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430134"
---
# <a name="windowsupdatestate-resource-type"></a>Ressourcentyp windowsUpdateState

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Noch nicht dokumentiert

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Dies ist die Id der Entität.|
|deviceId|Zeichenfolge|Die Id des Geräts.|
|userId|Zeichenfolge|Die Id des Benutzers.|
|deviceDisplayName|Zeichenfolge|Anzeigename des Geräts.|
|userPrincipalName|Zeichenfolge|Prinzipalnamen des Benutzers.|
|status|[WindowsUpdateStatus] (.. /Resources/Intune-deviceconfig-windowsupdatestatus.MD)|Windows Shapes-Status.|
|qualityUpdateVersion|Zeichenfolge|Die Qualität-Version des Geräts.|
|featureUpdateVersion|Zeichenfolge|Die aktuelle Feature Updateversion des Geräts.|
|lastScanDateTime|DateTimeOffset|Das Datum-Uhrzeit der Windows Update-Agent wurde erfolgreiche eine Überprüfung durch.|
|lastSyncDateTime|DateTimeOffset|Letzte Datum/Uhrzeit, die das Gerät mit Microsoft Intune mit synchronisieren.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.WindowsUpdateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.WindowsUpdateState",
  "id": "String (identifier)",
  "deviceId": "String (identifier)",
  "userId": "String (identifier)",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "status": "String",
  "qualityUpdateVersion": "String",
  "featureUpdateVersion": "String",
  "lastScanDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)"
}
```


