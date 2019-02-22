---
title: managedDeviceMobileAppConfiguration-Ressourcentyp
description: Eine abstrakte Klasse zur Konfiguration mobiler Apps für registrierte Geräte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dacccb00a30028a5b9e5144eb843ca52c60da876
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154250"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a>managedDeviceMobileAppConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Eine abstrakte Klasse zur Konfiguration mobiler Apps für registrierte Geräte.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedDeviceMobileAppConfigurations auflisten](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Objekte.|
|[managedDeviceMobileAppConfiguration abrufen](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)-Objekts.|
|[assign-Aktion](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität.|
|targetedMobileApps|String-Sammlung|Die zugeordnete App.|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese APP-Konfigurationsentität.|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts|
|description|Zeichenfolge|Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|displayName|Zeichenfolge|Vom Administrator bereitgestellter Name der Gerätekonfiguration|
|version|Int32|Version der Gerätekonfiguration.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)-Sammlung|Die Liste der Gruppenzuweisungen für die App-Konfiguration.|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Sammlung|Liste der ManagedDeviceMobileAppConfigurationDeviceStatus.|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)-Sammlung|Liste von ManagedDeviceMobileAppConfigurationUserStatus.|
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|Zusammenfassung der App-Konfiguration-Gerätestatus.|
|userStatusSummary|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|Zusammenfassung der App-Konfiguration-Benutzerstatus.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
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
  "version": 1024
}
```




