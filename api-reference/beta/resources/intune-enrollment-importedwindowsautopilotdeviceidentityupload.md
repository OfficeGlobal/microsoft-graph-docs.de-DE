---
title: importedWindowsAutopilotDeviceIdentityUpload-Ressourcentyp
description: Importieren Sie Windows Autopilot-Geräte mithilfe des Uploads.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ab6152a4347a7694e1ca6995fa683bda29b7206
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169636"
---
# <a name="importedwindowsautopilotdeviceidentityupload-resource-type"></a>importedWindowsAutopilotDeviceIdentityUpload-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Importieren Sie Windows Autopilot-Geräte mithilfe des Uploads.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[ImportedWindowsAutopilotDeviceIdentityUploads aufListen](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-list.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekte.|
|[ImportedWindowsAutopilotDeviceIdentityUpload abrufen](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-get.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|Lesen von Eigenschaften und Beziehungen des [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts.|
|[ImportedWindowsAutopilotDeviceIdentityUpload erstellen](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-create.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|Erstellen eines neuen [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts.|
|[ImportedWindowsAutopilotDeviceIdentityUpload löschen](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-delete.md)|Keine|Löscht eine [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).|
|[ImportedWindowsAutopilotDeviceIdentityUpload aktualisieren](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-update.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)|Aktualisieren der Eigenschaften eines [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) -Objekts.|
|[autopilotDeviceStream-Funktion](../api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream.md)|Zeichenfolge|Erstellen Sie eine Upload-Anforderung mit Autopilot-Gerätedaten Strom darin.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|GUID des Objekts|
|createdDateTimeUtc|DateTimeOffset|DateTime, wenn die Entität erstellt wird.|
|status|[importedWindowsAutopilotDeviceIdentityUploadStatus](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|Uploadstatus. Mögliche Werte: `noUpload`, `pending`, `complete`, `error`.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|deviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)-Sammlung|Sammlung aller Autopilot-Geräte als Teil dieses Uploads.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "String (identifier)",
  "createdDateTimeUtc": "String (timestamp)",
  "status": "String"
}
```




