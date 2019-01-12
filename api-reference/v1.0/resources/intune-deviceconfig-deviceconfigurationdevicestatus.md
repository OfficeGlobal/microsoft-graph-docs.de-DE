---
title: deviceConfigurationDeviceStatus-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6d4a04d2c4fc9a4a491351acd5bb5fd3caa42462
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949983"
---
# <a name="deviceconfigurationdevicestatus-resource-type"></a>deviceConfigurationDeviceStatus-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceConfigurationDeviceStatuses auflisten](../api/intune-deviceconfig-deviceconfigurationdevicestatus-list.md)|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Objekte.|
|[deviceConfigurationDeviceStatus abrufen](../api/intune-deviceconfig-deviceconfigurationdevicestatus-get.md)|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Lesen von Eigenschaften und Beziehungen des [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Objekts.|
|[deviceConfigurationDeviceStatus erstellen](../api/intune-deviceconfig-deviceconfigurationdevicestatus-create.md)|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Erstellen eines neuen [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Objekts.|
|[deviceConfigurationDeviceStatus löschen](../api/intune-deviceconfig-deviceconfigurationdevicestatus-delete.md)|Keine|Löscht ein [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Objekt.|
|[deviceConfigurationDeviceStatus aktualisieren](../api/intune-deviceconfig-deviceconfigurationdevicestatus-update.md)|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Aktualisieren der Eigenschaften eines [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|deviceDisplayName|Zeichenfolge|Gerätename, der dem Objekt des Typs „DevicePolicyStatus“ zugeordnet ist|
|userName|Zeichenfolge|Gemeldeter Benutzername|
|deviceModel|Zeichenfolge|Gemeldetes Gerätemodell|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Datum und Uhrzeit des Ablaufs der Toleranzperiode für die Gerätekonformität|
|status|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Konformitätsstatus des Richtlinienberichts. Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Richtlinienberichts|
|userPrincipalName|Zeichenfolge|Benutzer-Prinzipalname|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



