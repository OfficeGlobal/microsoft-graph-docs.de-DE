---
title: deviceManagementPartner-Ressourcentyp
description: Entität, die eine Verbindung mit dem Geräteverwaltungspartner darstellt.
ms.openlocfilehash: 46fd8f3ad06ea5b41bfcb1697b5826e1dd24a6b7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018678"
---
# <a name="devicemanagementpartner-resource-type"></a>deviceManagementPartner-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Entität, die eine Verbindung mit dem Geräteverwaltungspartner darstellt.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceManagementPartners auflisten](../api/intune-onboarding-devicemanagementpartner-list.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekte.|
|[deviceManagementPartner abrufen](../api/intune-onboarding-devicemanagementpartner-get.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Lesen von Eigenschaften und Beziehungen des [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekts.|
|[deviceManagementPartner erstellen](../api/intune-onboarding-devicemanagementpartner-create.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Erstellen eines neuen [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekts.|
|[deviceManagementPartner löschen](../api/intune-onboarding-devicemanagementpartner-delete.md)|Keine|Löscht ein [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekt.|
|[deviceManagementPartner aktualisieren](../api/intune-onboarding-devicemanagementpartner-update.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|Aktualisieren der Eigenschaften eines [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Noch nicht dokumentiert|
|lastHeartbeatDateTime|DateTimeOffset|Zeitstempel des letzten Heartbeats nach Aktivierung der Option „Connect to Device management Partner“ durch den Administrator|
|partnerState|[deviceManagementPartnerTenantState](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|Partner-Status, der diesen Mandanten. Mögliche Werte sind: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected` und `unresponsive`.|
|partnerAppType|[deviceManagementPartnerAppType](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|Partner-App-Typ. Mögliche Werte sind: `unknown`, `singleTenantApp` und `multiTenantApp`.|
|singleTenantAppId|String|ID der Partner-App mit einem einzelnen Mandanten|
|displayName|String|Anzeigename für Partner|
|isConfigured|Boolescher Wert|Gibt an, ob Geräteverwaltungspartner konfiguriert ist.|
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset|DateTime in UTC, zu der PartnerDevices entfernt werden|
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset|DateTime in UTC, zu der PartnerDevices als nicht kompatibel gekennzeichnet werden|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "String",
  "displayName": "String",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)"
}
```



