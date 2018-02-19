# <a name="managedapp-resource-type"></a>managedApp-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Abstrakte Klasse, die Eigenschaften und geerbte Eigenschaften für Apps enthält, die Sie mit einer Intune-App-Schutzrichtlinie verwalten können.

Erbt von [mobileApp](../resources/intune_apps_mobileapp.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[ManagedApps auflisten](../api/intune_apps_managedapp_list.md)|[managedApp](../resources/intune_apps_managedapp.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedApp](../resources/intune_apps_managedapp.md)-Objekte.|
|[ManagedApp abrufen](../api/intune_apps_managedapp_get.md)|[managedApp](../resources/intune_apps_managedapp.md)|Lesen von Eigenschaften und Beziehungen des [managedApp](../resources/intune_apps_managedapp.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|
|displayName|String|Der vom Administrator bereitgestellte oder importierte Titel der App. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|
|description|String|Die Beschreibung der App. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|
|publisher|String|Der Herausgeber der App. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune_apps_mimecontent.md)|Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der App. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der App. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|
|isFeatured|Boolean|Der Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md)|
|privacyInformationUrl|String|Die URL der Datenschutzbestimmungen. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|
|informationUrl|String|Die URL für weitere Informationen. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|
|owner|String|Der Besitzer der App. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|
|developer|String|Der Entwickler der App. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|
|notes|String|Hinweise für die App. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|
|publishingState|String|Der Veröffentlichungsstatus für die App. Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing`, `published`.|
|appAvailability|String|Die Verfügbarkeit der Anwendung. Mögliche Werte: `global`, `lineOfBusiness`.|
|version|String|Die Version der Anwendung.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)-Sammlung|Die Liste der Kategorien für diese App. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String",
  "appAvailability": "String",
  "version": "String"
}
```



