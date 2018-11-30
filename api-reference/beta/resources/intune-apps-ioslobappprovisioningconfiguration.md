---
title: Ressourcentyp iosLobAppProvisioningConfiguration
description: Dieses Thema enthält eine Beschreibung der deklarierte Methoden, Eigenschaften und Beziehungen, die von der Ressource IOS Branchen-App-Bereitstellung Konfiguration verfügbar gemacht werden.
ms.openlocfilehash: 07ae7c53f481aa6f2c9ad083881752591ab421fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062176"
---
# <a name="ioslobappprovisioningconfiguration-resource-type"></a>Ressourcentyp iosLobAppProvisioningConfiguration

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Dieses Thema enthält eine Beschreibung der deklarierte Methoden, Eigenschaften und Beziehungen, die von der Ressource IOS Branchen-App-Bereitstellung Konfiguration verfügbar gemacht werden.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste iosLobAppProvisioningConfigurations](../api/intune-apps-ioslobappprovisioningconfiguration-list.md)|[IosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Auflistung|Listeneigenschaften und Beziehungen der [IosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekte.|
|[Abrufen von iosLobAppProvisioningConfiguration](../api/intune-apps-ioslobappprovisioningconfiguration-get.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [IosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekts.|
|[Erstellen von iosLobAppProvisioningConfiguration](../api/intune-apps-ioslobappprovisioningconfiguration-create.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|Erstellen eines neuen [IosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekts.|
|[IosLobAppProvisioningConfiguration löschen](../api/intune-apps-ioslobappprovisioningconfiguration-delete.md)|Keines|Löscht eine [IosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).|
|[IosLobAppProvisioningConfiguration aktualisieren](../api/intune-apps-ioslobappprovisioningconfiguration-update.md)|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)|Aktualisieren Sie die Eigenschaften eines [IosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) -Objekts.|
|[assign-Aktion](../api/intune-apps-ioslobappprovisioningconfiguration-assign.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|expirationDateTime|DateTimeOffset|Optionales Profil Ablaufdatum und-Zeit.|
|payloadFileName|String|Der Dateiname (*.mobileprovision Nutzlast | *.xml)|
|payload|Binär|Nutzlast (UTF8-codiertes Bytearray)|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung des Objekts|
|description|String|Vom Administrator bereitgestellte Beschreibung der Gerätekonfiguration|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts.|
|displayName|String|Vom Administrator bereitgestellter Name der Gerätekonfiguration|
|version|Int32|Version der Gerätekonfiguration.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|groupAssignments|[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) -Auflistung|Die Zuordnungen zugeordneten Gruppe.|
|assignments|[IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) -Auflistung|Die zugeordneten Gruppe Zuordnungen für IosLobAppProvisioningConfiguration.|
|deviceStatuses|[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Auflistung|Die Liste der Geräte Installationsstatus für diese Konfiguration mobiler Apps.|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)-Sammlung|Die Liste der Benutzer des Installationsstatus für diese Konfiguration mobiler Apps.|

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





