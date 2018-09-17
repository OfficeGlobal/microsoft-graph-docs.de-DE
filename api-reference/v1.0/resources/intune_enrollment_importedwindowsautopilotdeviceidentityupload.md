# <a name="importedwindowsautopilotdeviceidentityupload-resource-type"></a>Ressourcentyp importedWindowsAutopilotDeviceIdentityUpload

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Importieren Sie Windows Autopilot-Geräte per Upload.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von importedWindowsAutopilotDeviceIdentityUploads](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_list.md)|[ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) -Objekte.|
|[Abrufen von importedWindowsAutopilotDeviceIdentityUpload](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_get.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)|Leseeigenschaften und Beziehungen des [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) -Objekts.|
|[Erstellen von importedWindowsAutopilotDeviceIdentityUpload](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_create.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)|Erstellen eines neuen [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) -Objekts.|
|[ImportedWindowsAutopilotDeviceIdentityUpload löschen](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_delete.md)|Keine|Löscht [ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md).|
|[importedWindowsAutopilotDeviceIdentityUpload aktualisieren](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_update.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)|Aktualisieren der Eigenschaften eines [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) -Objekts.|
|[autopilotDeviceStream-Funktion](../api/intune_enrollment_importedwindowsautopilotdeviceidentityupload_autopilotdevicestream.md)|Zeichenfolge|Erstellen einer Upload-Anfrage mit Autopilot-Gerätestream.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|GUID des Objekts|
|createdDateTimeUtc|DateTimeOffset|DateTime, wenn die Entität erstellt wird.|
|Status|[importedWindowsAutopilotDeviceIdentityUploadStatus](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityuploadstatus.md)|Upload-Status. Mögliche Werte: `noUpload`, `pending`, `complete`, `error`.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|deviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)-Sammlung|Sammlung aller Autopilot-Geräte als Teil dieses Uploads.|

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








