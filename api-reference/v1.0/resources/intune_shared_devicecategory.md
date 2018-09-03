# <a name="devicecategory-resource-type"></a>deviceCategory-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Gerätekategorien bieten eine Möglichkeit zum Organisieren Ihrer Geräte. Mithilfe von Gerätekategorien können Unternehmensadministratoren eigene Kategorien definieren, die für ihr Unternehmen sinnvoll sind. Diese Kategorien können dann in der Intune Azure-Konsole auf ein Gerät angewendet oder bei der Geräteregistrierung von einem Benutzer ausgewählt werden. Sie können basierend auf Gerätekategorien Berichte filtern und dynamische Azure Active Directory-Gerätegruppen erstellen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste DeviceCategories](../api/intune_shared_devicecategory_list.md) -Sammlung|Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceCategory](../resources/intune_shared_devicecategory.md) auf.|
|[deviceCategory abrufen](../api/intune_shared_devicecategory_get.md)|Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceCategory](../resources/intune_shared_devicecategory.md).|
|[deviceCategory erstellen](../api/intune_shared_devicecategory_create.md)|Erstellen eines neuen [deviceCategory](../resources/intune_shared_devicecategory.md)-Objekts.|
|[deviceCategory löschen](../api/intune_shared_devicecategory_delete.md).|
|[deviceCategory aktualisieren](../api/intune_shared_devicecategory_update.md)|Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceCategory](../resources/intune_shared_devicecategory.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für die Gerätekategorie. Schreibgeschützt.|
|**Onboarding**|
|displayName|Zeichenfolge|Der Anzeigename für die Gerätekategorie.|
|description|Zeichenfolge|Optionale Beschreibung für die Gerätekategorie.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```


