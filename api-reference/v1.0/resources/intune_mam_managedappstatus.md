# <a name="managedappstatus-resource-type"></a>managedAppStatus-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt den App-Schutz und den Konfigurationsstatus für die Organisation dar.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedAppStatuses auflisten](../api/intune_mam_managedappstatus_list.md)|[managedAppStatus](../resources/intune_mam_managedappstatus.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedAppStatus](../resources/intune_mam_managedappstatus.md)-Objekte.|
|[managedAppStatus abrufen](../api/intune_mam_managedappstatus_get.md)|[managedAppStatus](../resources/intune_mam_managedappstatus.md)|Lesen von Eigenschaften und Beziehungen des [managedAppStatus](../resources/intune_mam_managedappstatus.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Anzeigename des Statusberichts|
|id|Zeichenfolge|Schlüssel der Entität|
|Version|String|Version der Entität|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedAppStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



