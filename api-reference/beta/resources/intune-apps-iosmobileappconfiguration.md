---
title: iosMobileAppConfiguration-Ressourcentyp
description: Enthält Eigenschaften, geerbte Eigenschaften und Aktionen für Konfigurationen mobiler iOS-Apps.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 62d6355da2621ee86cabdea2d4a1edd3282ae98e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168656"
---
# <a name="iosmobileappconfiguration-resource-type"></a>iosMobileAppConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften, geerbte Eigenschaften und Aktionen für Konfigurationen mobiler iOS-Apps.


Erbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[iosMobileAppConfigurations auflisten](../api/intune-apps-iosmobileappconfiguration-list.md)|[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)-Objekte.|
|[iosMobileAppConfiguration abrufen](../api/intune-apps-iosmobileappconfiguration-get.md)|[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)-Objekts.|
|[iosMobileAppConfiguration erstellen](../api/intune-apps-iosmobileappconfiguration-create.md)|[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)|Erstellen eines neuen [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)-Objekts.|
|[iosMobileAppConfiguration löschen](../api/intune-apps-iosmobileappconfiguration-delete.md)|Keine|Löscht eine [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).|
|[iosMobileAppConfiguration aktualisieren](../api/intune-apps-iosmobileappconfiguration-update.md)|[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)|Aktualisieren der Eigenschaften eines [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität. Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|targetedMobileApps|String-Sammlung|Die zugeordnete App. Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese APP-Konfigurationsentität. Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts. Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|description|Zeichenfolge|Beschreibung der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|displayName|Zeichenfolge|Name der Gerätekonfiguration (vom Administrator festgelegt). Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|version|Int32|Version der Gerätekonfiguration. Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|encodedSettingXml|Binary|Base64-binärcodierte MDM-App-Konfiguration|
|Einstellungen|[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)-Sammlung|App-Konfigurationseinstellungselemente|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)-Sammlung|Die Liste der Gruppenzuweisungen für die App-Konfiguration. Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Sammlung|Liste der ManagedDeviceMobileAppConfigurationDeviceStatus. Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)-Sammlung|Liste von ManagedDeviceMobileAppConfigurationUserStatus. Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|Zusammenfassung der App-Konfiguration-Gerätestatus. Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|userStatusSummary|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|Zusammenfassung der App-Konfiguration-Benutzerstatus. Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosMobileAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "encodedSettingXml": "binary",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "String",
      "appConfigKeyType": "String",
      "appConfigKeyValue": "String"
    }
  ]
}
```




