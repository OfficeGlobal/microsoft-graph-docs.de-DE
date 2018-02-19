# <a name="deviceinstallstate-resource-type"></a>deviceInstallState-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für den Installationsstatus für ein Gerät.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceInstallStates auflisten](../api/intune_books_deviceinstallstate_list.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceInstallState](../resources/intune_books_deviceinstallstate.md)-Objekte.|
|[deviceInstallState abrufen](../api/intune_books_deviceinstallstate_get.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md)|Lesen von Eigenschaften und Beziehungen des [deviceInstallState](../resources/intune_books_deviceinstallstate.md)-Objekts.|
|[deviceInstallState erstellen](../api/intune_books_deviceinstallstate_create.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md)|Erstellen eines neuen [deviceInstallState](../resources/intune_books_deviceinstallstate.md)-Objekts.|
|[deviceInstallState löschen](../api/intune_books_deviceinstallstate_delete.md)|Keine|Löscht ein [deviceInstallState](../resources/intune_books_deviceinstallstate.md)-Objekt.|
|[deviceInstallState aktualisieren](../api/intune_books_deviceinstallstate_update.md)|[deviceInstallState](../resources/intune_books_deviceinstallstate.md)|Aktualisieren der Eigenschaften eines [deviceInstallState](../resources/intune_books_deviceinstallstate.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität.|
|deviceName|String|Gerätename|
|deviceId|String|Geräte-ID|
|lastSyncDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Synchronisierung|
|installState|String|Der Installationsstatus des E-Books. Mögliche Werte: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.|
|errorCode|String|Der Fehlercode für Fehler bei der Installation.|
|osVersion|String|Betriebssystemversion|
|osDescription|String|Beschreibung des Betriebssystems|
|userName|String|Benutzername des Geräts|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```



