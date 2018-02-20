# <a name="managedappstatusraw-resource-type"></a>managedAppStatusRaw-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.

Erbt von [managedAppStatus](../resources/intune_mam_managedappstatus.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedAppStatusRaws auflisten](../api/intune_mam_managedappstatusraw_list.md)|[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)-Objekte.|
|[ManagedAppStatusRaw abrufen](../api/intune_mam_managedappstatusraw_get.md)|[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)|Lesen von Eigenschaften und Beziehungen des [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)-Objekts.|
|[ManagedAppStatusRaw erstellen](../api/intune_mam_managedappstatusraw_create.md)|[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)|Erstellen eines neuen [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)-Objekts.|
|[ManagedAppStatusRaw löschen](../api/intune_mam_managedappstatusraw_delete.md)|Keine|Löscht ein [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)-Objekt.|
|[ManagedAppStatusRaw aktualisieren](../api/intune_mam_managedappstatusraw_update.md)|[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)|Aktualisieren der Eigenschaften eines [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Anzeigename des Statusberichts. Geerbt von [managedAppStatus](../resources/intune_mam_managedappstatus.md)|
|id|String|Schlüssel der Entität. Geerbt von [managedAppStatus](../resources/intune_mam_managedappstatus.md)|
|version|String|Version der Entität Geerbt von [managedAppStatus](../resources/intune_mam_managedappstatus.md)|
|content|[Json](../resources/intune_mam_json.md)|Inhalt des Statusberichts.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```


