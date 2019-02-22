---
title: deviceManagementScriptRunSummary-Ressourcentyp
description: Enthält Eigenschaften für die Ausführungs Zusammenfassung eines Geräteverwaltungsskripts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3fe26fc121d0d1d9339de999101975d2c4c225a5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174270"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a>deviceManagementScriptRunSummary-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften für die Ausführungs Zusammenfassung eines Geräteverwaltungsskripts.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[DeviceManagementScriptRunSummary abrufen](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekts.|
|[DeviceManagementScriptRunSummary aktualisieren](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|Aktualisieren der Eigenschaften eines [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Der Schlüssel der Device Management-Skript Ausführungs Zusammenfassungs Entität.|
|successDeviceCount|Int32|Anzahl der erfolgreichen Geräte.|
|errorDeviceCount|Int32|Fehlergeräte Anzahl.|
|successUserCount|Int32|Anzahl der erfolgreichen Benutzer.|
|errorUserCount|Int32|Fehler Benutzeranzahl.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```




