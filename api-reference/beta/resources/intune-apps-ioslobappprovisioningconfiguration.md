---
title: iosLobAppProvisioningConfiguration-Ressourcentyp
description: Dieses Thema enthält Beschreibungen der deklarierten Methoden, Eigenschaften und Beziehungen, die von der Konfigurationsressource für die IOS-Branchen-App bereitgestellt werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ab481571cce9bd986b31d12c41705f8fb48558b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151037"
---
# <a name="ioslobappprovisioningconfiguration-resource-type"></a>iosLobAppProvisioningConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Dieses Thema enthält Beschreibungen der deklarierten Methoden, Eigenschaften und Beziehungen, die von der Konfigurationsressource für die IOS-Branchen-App bereitgestellt werden.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[IosLobAppProvisioningConfigurations aufListen](../api/intune-apps-ioslobappprovisioningconfiguration-list.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekte.|
|[IosLobAppProvisioningConfiguration abrufen](../api/intune-apps-ioslobappprovisioningconfiguration-get.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekts.|
|[IosLobAppProvisioningConfiguration erstellen](../api/intune-apps-ioslobappprovisioningconfiguration-create.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|Erstellen eines neuen [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekts.|
|[IosLobAppProvisioningConfiguration löschen](../api/intune-apps-ioslobappprovisioningconfiguration-delete.md)|Keine|Löscht eine [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).|
|[IosLobAppProvisioningConfiguration aktualisieren](../api/intune-apps-ioslobappprovisioningconfiguration-update.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|Aktualisieren der Eigenschaften eines [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekts.|
|[assign-Aktion](../api/intune-apps-ioslobappprovisioningconfiguration-assign.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität|
|expirationDateTime|DateTimeOffset|Optionales Profil Ablaufdatum und-Uhrzeit.|
|payloadFileName|Zeichenfolge|Name der Nutzlastdatei (*. mobileprovision | *.xml)|
|payload|Binär|Nutzlast (UTF8-codiertes Bytearray)|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts|
|description|String|Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|displayName|Zeichenfolge|Vom Administrator bereitgestellter Name der Gerätekonfiguration|
|version|Int32|Version der Gerätekonfiguration.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Sammlung|Die zugeordneten Gruppenzuweisungen.|
|assignments|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Sammlung|Die zugeordneten Gruppenzuweisungen für IosLobAppProvisioningConfiguration.|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Sammlung|Die Liste der Geräte Installationsstatus für diese Konfiguration für Mobile Apps.|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)-Sammlung|Die Liste der Benutzer Installationsstatus für diese Konfiguration für Mobile Apps.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobAppProvisioningConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "String (identifier)",
  "expirationDateTime": "String (timestamp)",
  "payloadFileName": "String",
  "payload": "binary",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```




