---
title: settingStateDeviceSummary-Ressourcentyp
description: Zusammenfassung des Zustands der Gerätekonformitätsrichtlinien und -konfigurations-Einstellung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3c36b4270896716b6fdb7de11a35b5267ed5d16
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163679"
---
# <a name="settingstatedevicesummary-resource-type"></a>settingStateDeviceSummary-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Zusammenfassung des Zustands der Gerätekonformitätsrichtlinien und -konfigurations-Einstellung

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[settingStateDeviceSummaries auflisten](../api/intune-deviceconfig-settingstatedevicesummary-list.md)| [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Objekte.|
|[settingStateDeviceSummary abrufen](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Lesen von Eigenschaften und Beziehungen des [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Objekts.|
|[settingStateDeviceSummary erstellen](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Erstellen eines neuen [SettingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Objekts.|
|[settingStateDeviceSummary löschen](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|Keine|Löscht eine [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).|
|[settingStateDeviceSummary aktualisieren](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Aktualisieren der Eigenschaften eines [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|settingName|Zeichenfolge|Name der Einstellung|
|instancePath|Zeichenfolge|Name des zur Einstellung gehörenden Objekts des Typs „InstancePath“|
|unknownDeviceCount|Int32|Anzahl der Geräte mit Meldung „Unknown“ für die Einstellung|
|notApplicableDeviceCount|Int32|Anzahl der Geräte mit Meldung „Not Applicable“ für die Einstellung|
|compliantDeviceCount|Int32|Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung|
|remediatedDeviceCount|Int32|Anzahl der Geräte mit Meldung „Compliant“ für die Einstellung|
|nonCompliantDeviceCount|Int32|Anzahl der Geräte mit Meldung „NonCompliant“ für die Einstellung|
|errorDeviceCount|Int32|Anzahl der Geräte mit Meldung „Error“ für die Einstellung|
|conflictDeviceCount|Int32|Anzahl der Geräte mit Konfliktfehler für die Einstellung|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.settingStateDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "instancePath": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```




