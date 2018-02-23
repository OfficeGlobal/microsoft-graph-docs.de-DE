# <a name="androidlobapp-resource-type"></a>androidLobApp-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften und geerbte Eigenschaften für branchenspezifische Android-Apps.

Erbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[AndroidLobApps auflisten](../api/intune_apps_androidlobapp_list.md)|[androidLobApp](../resources/intune_apps_androidlobapp.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [androidLobApp](../resources/intune_apps_androidlobapp.md)-Objekte.|
|[AndroidLobApp abrufen](../api/intune_apps_androidlobapp_get.md)|[androidLobApp](../resources/intune_apps_androidlobapp.md)|Lesen von Eigenschaften und Beziehungen des [androidLobApp](../resources/intune_apps_androidlobapp.md)-Objekts.|
|[AndroidLobApp erstellen](../api/intune_apps_androidlobapp_create.md)|[androidLobApp](../resources/intune_apps_androidlobapp.md)|Erstellen eines neuen [androidLobApp](../resources/intune_apps_androidlobapp.md)-Objekts.|
|[AndroidLobApp löschen](../api/intune_apps_androidlobapp_delete.md)|Keine|Löscht ein [androidLobApp](../resources/intune_apps_androidlobapp.md)-Objekt.|
|[AndroidLobApp aktualisieren](../api/intune_apps_androidlobapp_update.md)|[androidLobApp](../resources/intune_apps_androidlobapp.md)|Aktualisieren der Eigenschaften eines [androidLobApp](../resources/intune_apps_androidlobapp.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|displayName|String|Der vom Administrator bereitgestellte oder importierte Titel der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|description|String|Beschreibung der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|publisher|String|Der Herausgeber der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune_apps_mimecontent.md)|Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|isFeatured|Boolean|Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|privacyInformationUrl|String|URL zur Datenschutzerklärung. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|informationUrl|String|URL zur Seite mit weiteren Informationen. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|owner|String|Der Besitzer der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|developer|String|Der Entwickler der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|notes|String|Hinweise für die App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|publishingState|String|Der Veröffentlichungsstatus für die App. Die App kann nicht zugewiesen werden, solange sie nicht veröffentlicht wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.|
|committedContentVersion|String|Die interne zugesicherte Inhaltsversion. Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|
|fileName|String|Der Name der Hauptdatei der Branchenanwendung. Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|
|size|Int64|Die Gesamtgröße einschließlich aller hochgeladenen Dateien. Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|
|packageId|String|Der Paketbezeichner|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune_apps_androidminimumoperatingsystem.md)|Der Wert für die Mindestversion des verwendbaren Betriebssystems|
|versionName|String|Der Versionsname der branchenspezifischen Android-App.|
|versionCode|String|Der Versionscode der branchenspezifischen Android-App.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Die Liste der Kategorien für diese App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|assignments|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|contentVersions|Sammlung von Objekten des Typs [mobileAppContent](../resources/intune_apps_mobileappcontent.md)|Die Liste der Inhaltsversionen für diese App. Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "packageId": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "String",
  "versionCode": "String"
}
```



