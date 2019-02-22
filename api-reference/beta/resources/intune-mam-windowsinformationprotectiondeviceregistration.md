---
title: windowsInformationProtectionDeviceRegistration-Ressourcentyp
description: Stellt Geräte Registrierungsdatensätze für BYOD-Windows-Geräte (Bring-your-own-Device) dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d4403ae2e4629a330fadd5136530d66c8a7d7f2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161677"
---
# <a name="windowsinformationprotectiondeviceregistration-resource-type"></a>windowsInformationProtectionDeviceRegistration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt Geräte Registrierungsdatensätze für BYOD-Windows-Geräte (Bring-your-own-Device) dar.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsInformationProtectionDeviceRegistrations aufListen](../api/intune-mam-windowsinformationprotectiondeviceregistration-list.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Objekte.|
|[WindowsInformationProtectionDeviceRegistration abrufen](../api/intune-mam-windowsinformationprotectiondeviceregistration-get.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Lesen von Eigenschaften und Beziehungen des [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Objekts.|
|[WindowsInformationProtectionDeviceRegistration erstellen](../api/intune-mam-windowsinformationprotectiondeviceregistration-create.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Erstellen eines neuen [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Objekts.|
|[WindowsInformationProtectionDeviceRegistration löschen](../api/intune-mam-windowsinformationprotectiondeviceregistration-delete.md)|Keine|Löscht eine [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).|
|[WindowsInformationProtectionDeviceRegistration aktualisieren](../api/intune-mam-windowsinformationprotectiondeviceregistration-update.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Aktualisieren der Eigenschaften eines [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Objekts.|
|[wipe-Aktion](../api/intune-mam-windowsinformationprotectiondeviceregistration-wipe.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|userId|Zeichenfolge|ID, die diesem Geräte Registrierungseintrag zugeordnet ist.|
|deviceRegistrationId|String|Gerätebezeichner für diesen Geräte Registrierungseintrag.|
|deviceName|Zeichenfolge|Name des Geräts|
|deviceType|Zeichenfolge|Gerätetyp, beispielsweise Windows Laptop und Windows phone.|
|deviceMacAddress|Zeichenfolge|Mac-Adresse des Geräts.|
|lastCheckInDateTime|DateTimeOffset|Zeitpunkt des letzten Eincheckens des Geräts.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDeviceRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "String (identifier)",
  "userId": "String",
  "deviceRegistrationId": "String",
  "deviceName": "String",
  "deviceType": "String",
  "deviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```




