---
title: Ressourcentyp windowsInformationProtectionDeviceRegistration
description: Stellt Gerät Registrierung Einträge für Bring-Your-Own-Device(BYOD) Windows-Geräte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ae81d973db8c47d9fa613db0eb1b661bb8fa0f9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430044"
---
# <a name="windowsinformationprotectiondeviceregistration-resource-type"></a>Ressourcentyp windowsInformationProtectionDeviceRegistration

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Stellt Gerät Registrierung Einträge für Bring-Your-Own-Device(BYOD) Windows-Geräte.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste windowsInformationProtectionDeviceRegistrations](../api/intune-mam-windowsinformationprotectiondeviceregistration-list.md)|[WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Auflistung|Listeneigenschaften und Beziehungen der [WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Objekte.|
|[Abrufen von windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-get.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Lesen Sie Eigenschaften und Beziehungen des [WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Objekts.|
|[Erstellen von windowsInformationProtectionDeviceRegistration](../api/intune-mam-windowsinformationprotectiondeviceregistration-create.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Erstellen eines neuen [WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Objekts.|
|[WindowsInformationProtectionDeviceRegistration löschen](../api/intune-mam-windowsinformationprotectiondeviceregistration-delete.md)|Keine|Löscht eine [WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).|
|[WindowsInformationProtectionDeviceRegistration aktualisieren](../api/intune-mam-windowsinformationprotectiondeviceregistration-update.md)|[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)|Aktualisieren Sie die Eigenschaften eines [WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) -Objekts.|
|[wipe-Aktion](../api/intune-mam-windowsinformationprotectiondeviceregistration-wipe.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|userId|Zeichenfolge|Benutzer-ID dieses Gerät registrierungsdatensatzes zugeordnet.|
|deviceRegistrationId|String|Geräte-ID für dieses Gerät registrierungsdatensatzes.|
|deviceName|String|Name des Geräts|
|deviceType|Zeichenfolge|Gerätetyp, beispielsweise Windows Laptop VS Windows Phone.|
|deviceMacAddress|Zeichenfolge|Mac-Adresse des Geräts.|
|lastCheckInDateTime|DateTimeOffset|Zeitpunkt der letzten Einchecken des Geräts.|

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




