---
title: Ressourcentyp managedDeviceMobileAppConfigurationDeviceStatus
description: Enthält Eigenschaften, geerbten Eigenschaften und Aktionen für die Konfigurationsstatus für eine MDM mobile app bei einem Gerät.
ms.openlocfilehash: 07a8d18c7d7ab09b2dd824e4d32576fbbdb7ecc5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063512"
---
# <a name="manageddevicemobileappconfigurationdevicestatus-resource-type"></a>Ressourcentyp managedDeviceMobileAppConfigurationDeviceStatus

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften, geerbten Eigenschaften und Aktionen für die Konfigurationsstatus für eine MDM mobile app bei einem Gerät.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste managedDeviceMobileAppConfigurationDeviceStatuses](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-list.md)|[ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Auflistung|Listeneigenschaften und Beziehungen der [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekte.|
|[Abrufen von managedDeviceMobileAppConfigurationDeviceStatus](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-get.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|Lesen Sie Eigenschaften und Beziehungen des [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekts.|
|[Erstellen von managedDeviceMobileAppConfigurationDeviceStatus](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-create.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|Erstellen eines neuen [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekts.|
|[ManagedDeviceMobileAppConfigurationDeviceStatus löschen](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-delete.md)|Keines|Löscht eine [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).|
|[ManagedDeviceMobileAppConfigurationDeviceStatus aktualisieren](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-update.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|Aktualisieren Sie die Eigenschaften eines [ManagedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|deviceDisplayName|String|Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist|
|userName|String|Gemeldeter Benutzername|
|deviceModel|String|Gemeldetes Gerätemodell|
|Plattform|Int32|Plattform des Geräts, das gemeldet wird|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität|
|status|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Konformitätsstatus des Richtlinienberichts. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Richtlinienberichts|
|userPrincipalName|String|Benutzer-Prinzipalname|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "platform": 1024,
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```





