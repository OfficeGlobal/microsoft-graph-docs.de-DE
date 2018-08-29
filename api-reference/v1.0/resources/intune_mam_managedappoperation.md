# <a name="managedappoperation-resource-type"></a>managedAppOperation-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Steht für einen Vorgang, der auf eine App-Registrierung angewendet wird.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedAppOperations auflisten](../api/intune_mam_managedappoperation_list.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedAppOperation](../resources/intune_mam_managedappoperation.md)-Objekte.|
|[managedAppOperation abrufen](../api/intune_mam_managedappoperation_get.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)|Lesen von Eigenschaften und Beziehungen des [managedAppOperation](../resources/intune_mam_managedappoperation.md)-Objekts.|
|[managedAppOperation erstellen](../api/intune_mam_managedappoperation_create.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)|Erstellen eines neuen [managedAppOperation](../resources/intune_mam_managedappoperation.md)-Objekts.|
|[managedAppOperation löschen](../api/intune_mam_managedappoperation_delete.md)|Keine|Löscht ein [managedAppOperation](../resources/intune_mam_managedappoperation.md)-Objekt.|
|[managedAppOperation aktualisieren](../api/intune_mam_managedappoperation_update.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)|Aktualisieren der Eigenschaften eines [managedAppOperation](../resources/intune_mam_managedappoperation.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Name des Vorgangs|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des App-Vorgangs|
|state|String|Aktueller Status des Vorgangs|
|id|Zeichenfolge|Schlüssel der Entität|
|Version|String|Version der Entität|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedAppOperation"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



