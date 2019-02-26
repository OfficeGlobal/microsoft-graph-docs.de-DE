---
title: iosCustomConfiguration-Ressourcentyp
description: Dieses Thema enthält eine Beschreibung der deklarierten Methoden, Eigenschaften und Beziehungen, die von der Ressource iosCustomConfiguration verfügbar gemacht werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a91515ddfcbc4932e9615d8253097549f69773b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252840"
---
# <a name="ioscustomconfiguration-resource-type"></a>iosCustomConfiguration-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Dieses Thema enthält eine Beschreibung der deklarierten Methoden, Eigenschaften und Beziehungen, die von der Ressource iosCustomConfiguration verfügbar gemacht werden.


Sie erbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[iosCustomConfigurations auflisten](../api/intune-deviceconfig-ioscustomconfiguration-list.md)|[iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md)-Objekte.|
|[iosCustomConfiguration abrufen](../api/intune-deviceconfig-ioscustomconfiguration-get.md)|[iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md)-Objekts.|
|[iosCustomConfiguration erstellen](../api/intune-deviceconfig-ioscustomconfiguration-create.md)|[iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md)|Erstellen eines neuen [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md)-Objekts.|
|[iosCustomConfiguration löschen](../api/intune-deviceconfig-ioscustomconfiguration-delete.md)|Keine|Löscht eine [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).|
|[iosCustomConfiguration aktualisieren](../api/intune-deviceconfig-ioscustomconfiguration-update.md)|[iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md)|Aktualisieren der Eigenschaften eines [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Version|Int32|Version der Gerätekonfiguration. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|payloadName|Zeichenfolge|Name, der dem Benutzer angezeigt wird|
|payloadFileName|Zeichenfolge|Name der Nutzlastdatei (*.mobileconfig | *.xml)|
|payload|Binär|Nutzlast (UTF8-codiertes Bytearray)|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)-Sammlung|Liste der Zuweisungen für das Gerätekonfigurationsprofil. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)-Sammlung|Installationsstatus der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Übersicht über den Status der Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Übersicht über den Status der Gerätekonfiguration nach Benutzer. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries| [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)-Sammlung|Übersicht über den Einstellungsstatus für die Gerätekonfiguration nach Gerät. Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosCustomConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "payloadName": "String",
  "payloadFileName": "String",
  "payload": "binary"
}
```



