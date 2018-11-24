# <a name="mobileappcontentfile-resource-type"></a>mobileAppContentFile-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für eine einzelne Installationsdatei, die mit einer bestimmten mobileAppContent-Version verknüpft ist.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[MobileAppContentFiles auflisten](../api/intune_apps_mobileappcontentfile_list.md)|[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)-Objekte.|
|[MobileAppContentFile abrufen](../api/intune_apps_mobileappcontentfile_get.md)|[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)|Lesen von Eigenschaften und Beziehungen des [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)-Objekts.|
|[MobileAppContentFile erstellen](../api/intune_apps_mobileappcontentfile_create.md)|[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)|Erstellen eines neuen [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)-Objekts.|
|[MobileAppContentFile löschen](../api/intune_apps_mobileappcontentfile_delete.md)|Keine|Löscht ein [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)-Objekt.|
|[MobileAppContentFile aktualisieren](../api/intune_apps_mobileappcontentfile_update.md)|[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)|Aktualisieren der Eigenschaften eines [MobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)-Objekts.|
|[commit-Aktion](../api/intune_apps_mobileappcontentfile_commit.md)|Keine|Führt einen Commit für eine Datei einer bestimmten App aus.|
|[renewUpload-Aktion](../api/intune_apps_mobileappcontentfile_renewupload.md)|Keine|Erneuert den SAS-URI für einen Anwendungsdateiupload.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|azureStorageUri|String|Der Azure Storage-URI.|
|isCommitted|Boolean|Ein Wert, der angibt, ob für die Datei ein Commit ausgeführt wurde.|
|id|String|Die Datei-ID|
|createdDateTime|DateTimeOffset|Der Zeitpunkt der Erstellung der Datei|
|name|String|Der Dateiname|
|size|Int64|Die Größe der Datei vor der Verschlüsselung.|
|sizeEncrypted|Int64|Die Größe der Datei nach der Verschlüsselung.|
|azureStorageUriExpirationDateTime|DateTimeOffset|Die Zeit, zu der der Azure Storage-URI abläuft.|
|manifest|Binary|Die Manifestinformationen|
|uploadState|[mobileAppContentFileUploadState](../resources/intune_apps_mobileappcontentfileuploadstate.md)|Status der aktuellen Uploadanforderung. Mögliche Werte sind: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContentFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "String",
  "isCommitted": true,
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "sizeEncrypted": 1024,
  "azureStorageUriExpirationDateTime": "String (timestamp)",
  "manifest": "binary",
  "uploadState": "String"
}
```



