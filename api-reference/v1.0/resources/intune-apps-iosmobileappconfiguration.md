---
title: iosMobileAppConfiguration-Ressourcentyp
description: Enthält Eigenschaften, geerbte Eigenschaften und Aktionen für Konfigurationen mobiler iOS-Apps.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: aff33ae97d883e2fcd238d54b1a66ff0dd6e8b90
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925959"
---
# <a name="iosmobileappconfiguration-resource-type"></a>iosMobileAppConfiguration-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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
|id|Zeichenfolge|Schlüssel der Entität. Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
|targetedMobileApps|String-Sammlung|Die zugeordnete App. Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
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
|deviceStatuses|[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Auflistung|Liste der ManagedDeviceMobileAppConfigurationDeviceStatus. Geerbt von [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|
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



