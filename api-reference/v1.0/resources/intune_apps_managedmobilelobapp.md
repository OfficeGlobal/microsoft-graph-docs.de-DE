# <a name="managedmobilelobapp-resource-type"></a>managedMobileLobApp-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine abstrakte Basisklasse mit Eigenschaften für alle verwalteten mobilen branchenspezifischen Apps.

Erbt von [managedApp](../resources/intune_apps_managedapp.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[ManagedMobileLobApps auflisten](../api/intune_apps_managedmobilelobapp_list.md)|[managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)-Objekte.|
|[ManagedMobileLobApp abrufen](../api/intune_apps_managedmobilelobapp_get.md)|[managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)|Lesen von Eigenschaften und Beziehungen des [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md)-Objekts.|

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
|appAvailability|String|Die Verfügbarkeit der Anwendung. Geerbt von [managedApp](../resources/intune_apps_managedapp.md). Mögliche Werte sind: `global`, `lineOfBusiness`.|
|version|String|Die Version der Anwendung. Geerbt von [managedApp](../resources/intune_apps_managedapp.md)|
|committedContentVersion|String|Die interne zugesicherte Inhaltsversion.|
|fileName|String|Der Name der Hauptdatei der Branchenanwendung|
|size|Int64|Die Gesamtgröße einschließlich aller hochgeladenen Dateien|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)-Sammlung|Die Liste der Kategorien für diese App. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/intune_apps_mobileappcontent.md)-Sammlung|Die Liste der Inhaltsversionen für diese App.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileLobApp",
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
  "version": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024
}
```



