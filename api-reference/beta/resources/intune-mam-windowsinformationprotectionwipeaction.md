---
title: windowsInformationProtectionWipeAction-Ressourcentyp
description: Stellt Löschanforderungen dar, die vom mandantenadministrator für BYOD-Windows-Geräte (Bring-your-own-Device) ausgestellt wurden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e08cd6a2cf27830f6f88328440fb100bcd77ef6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148006"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a>windowsInformationProtectionWipeAction-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt Löschanforderungen dar, die vom mandantenadministrator für BYOD-Windows-Geräte (Bring-your-own-Device) ausgestellt wurden.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[WindowsInformationProtectionWipeActions aufListen](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekte.|
|[WindowsInformationProtectionWipeAction abrufen](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Lesen von Eigenschaften und Beziehungen des [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekts.|
|[WindowsInformationProtectionWipeAction erstellen](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Erstellen eines neuen [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekts.|
|[WindowsInformationProtectionWipeAction löschen](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|Keine|Löscht eine [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).|
|[WindowsInformationProtectionWipeAction aktualisieren](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Aktualisieren der Eigenschaften eines [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|status|[actionState](../resources/intune-shared-actionstate.md)|Aktionsstatus wischen. Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.|
|targetedUserId|Zeichenfolge|Die UserId, die von dieser Löschaktion bestimmt wird.|
|targetedDeviceRegistrationId|Zeichenfolge|Die DeviceRegistrationId, die von dieser Löschaktion bestimmt wird.|
|targetedDeviceName|Zeichenfolge|Name des Zielgeräts.|
|targetedDeviceMacAddress|Zeichenfolge|Mac-Adresse des Zielgeräts.|
|lastCheckInDateTime|DateTimeOffset|Letzter Eincheck Zeitpunkt des Geräts, das von dieser Löschaktion bestimmt wurde.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionWipeAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "String (identifier)",
  "status": "String",
  "targetedUserId": "String",
  "targetedDeviceRegistrationId": "String",
  "targetedDeviceName": "String",
  "targetedDeviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```




