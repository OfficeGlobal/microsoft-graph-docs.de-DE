# <a name="mobileappcategory-resource-type"></a>mobileAppCategory-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften für eine einzelne Intune-App-Kategorie.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[mobileAppCategories auflisten](../api/intune_apps_mobileappcategory_list.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)-Objekte.|
|[mobileAppCategory abrufen](../api/intune_apps_mobileappcategory_get.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Lesen von Eigenschaften und Beziehungen des [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)-Objekts.|
|[mobileAppCategory erstellen](../api/intune_apps_mobileappcategory_create.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Erstellen eines neuen [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)-Objekts.|
|[MobileAppCategory löschen](../api/intune_apps_mobileappcategory_delete.md)|Keine|Löscht eine [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).|
|[mobileAppCategory aktualisieren](../api/intune_apps_mobileappcategory_update.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Aktualisieren der Eigenschaften eines [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|String|Schlüssel der Entität|
|displayName|String|Name der App-Kategorie|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der mobileAppCategory.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```








