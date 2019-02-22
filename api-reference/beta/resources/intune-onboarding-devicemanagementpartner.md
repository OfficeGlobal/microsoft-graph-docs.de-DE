---
title: deviceManagementPartner-Ressourcentyp
description: Entität, die eine Verbindung mit dem Geräteverwaltungspartner darstellt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5d76eaa160783297208bfd25f3d898a562b59c1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139641"
---
# <a name="devicemanagementpartner-resource-type"></a>deviceManagementPartner-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|id|Zeichenfolge|ID der Entität|
|lastHeartbeatDateTime|DateTimeOffset|Zeitstempel des letzten Heartbeats nach Aktivierung der Option „Connect to Device management Partner“ durch den Administrator|
|partnerState|[deviceManagementPartnerTenantState](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|Partner Status dieses Mandanten. Mögliche Werte sind: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected` und `unresponsive`.|
|partnerAppType|[deviceManagementPartnerAppType](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|Partner-App-Typ. Mögliche Werte sind: `unknown`, `singleTenantApp` und `multiTenantApp`.|
|singleTenantAppId|String|ID der Partner-App mit einem einzelnen Mandanten|
|displayName|Zeichenfolge|Anzeigename für Partner|
|isConfigured|Boolescher Wert|Gibt an, ob Geräteverwaltungspartner konfiguriert ist.|
|whenPartnerDevicesWillBeRemoved|DateTimeOffset|DateTime in UTC, wenn PartnerDevices entfernt wird. Dies wird bald Obselete.|
|whenPartnerDevicesWillBeMarkedAsNonCompliant|DateTimeOffset|DateTime in UTC, wenn PartnerDevices als nicht kompatibel gekennzeichnet wird. Dies wird bald Obselete.|
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
  "whenPartnerDevicesWillBeRemoved": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "String (timestamp)",
  "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)"
}
```




