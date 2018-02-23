# <a name="devicecategory-resource-type"></a>deviceCategory-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Gerätekategorien bieten eine Möglichkeit zum Organisieren Ihrer Geräte. Mithilfe von Gerätekategorien können Unternehmensadministratoren eigene Kategorien definieren, die für ihr Unternehmen sinnvoll sind. Diese Kategorien können dann in der Intune Azure-Konsole auf ein Gerät angewendet oder bei der Geräteregistrierung von einem Benutzer ausgewählt werden. Sie können basierend auf Gerätekategorien Berichte filtern und dynamische Azure Active Directory-Gerätegruppen erstellen.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceCategories auflisten](../api/intune_onboarding_devicecategory_list.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceCategory](../resources/intune_onboarding_devicecategory.md)-Objekte.|
|[deviceCategory abrufen](../api/intune_onboarding_devicecategory_get.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md)|Lesen von Eigenschaften und Beziehungen des [deviceCategory](../resources/intune_onboarding_devicecategory.md)-Objekts.|
|[deviceCategory erstellen](../api/intune_onboarding_devicecategory_create.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md)|Erstellen eines neuen [deviceCategory](../resources/intune_onboarding_devicecategory.md)-Objekts.|
|[deviceCategory löschen](../api/intune_onboarding_devicecategory_delete.md)|Keine|Löscht ein [deviceCategory](../resources/intune_onboarding_devicecategory.md)-Objekt.|
|[deviceCategory aktualisieren](../api/intune_onboarding_devicecategory_update.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md)|Aktualisieren der Eigenschaften eines [deviceCategory](../resources/intune_onboarding_devicecategory.md)-Objekts|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Der eindeutige Bezeichner für die Gerätekategorie. Schreibgeschützt.|
|displayName|String|Der Anzeigename für die Gerätekategorie.|
|description|String|Optionale Beschreibung für die Gerätekategorie.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



