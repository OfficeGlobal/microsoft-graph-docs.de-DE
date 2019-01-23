---
title: Ressourcentyp windowsInformationProtectionWipeAction
description: Stellt Wischen Anforderungen einstufen der mandantenadministrator für Bring-Your-Own-Device(BYOD) Windows-Geräte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 67af8bdde412381bb6362ef1768dca12fdfce6c2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431565"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a>Ressourcentyp windowsInformationProtectionWipeAction

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Stellt Wischen Anforderungen einstufen der mandantenadministrator für Bring-Your-Own-Device(BYOD) Windows-Geräte.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste windowsInformationProtectionWipeActions](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|[WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Auflistung|Listeneigenschaften und Beziehungen der [WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekte.|
|[Abrufen von windowsInformationProtectionWipeAction](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Lesen Sie Eigenschaften und Beziehungen des [WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekts.|
|[Erstellen von windowsInformationProtectionWipeAction](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Erstellen eines neuen [WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekts.|
|[WindowsInformationProtectionWipeAction löschen](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|Keine|Löscht eine [WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).|
|[WindowsInformationProtectionWipeAction aktualisieren](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|Aktualisieren Sie die Eigenschaften eines [WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|status|[actionState](../resources/intune-shared-actionstate.md)|Wischen Sie Aktionsstatus. Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.|
|targetedUserId|Zeichenfolge|Die Benutzer-ID, die diese Aktion Remotegerätzurücksetzung darstellt.|
|targetedDeviceRegistrationId|Zeichenfolge|Die DeviceRegistrationId diese Aktion Remotegerätzurücksetzung darstellt.|
|targetedDeviceName|Zeichenfolge|Gezielte Gerätename.|
|targetedDeviceMacAddress|Zeichenfolge|Zielgerät Mac-Adresse.|

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
  "targetedDeviceMacAddress": "String"
}
```




