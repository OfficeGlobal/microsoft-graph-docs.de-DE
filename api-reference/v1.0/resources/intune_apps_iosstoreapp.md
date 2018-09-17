# <a name="iosstoreapp-resource-type"></a>iosStoreApp-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enthält Eigenschaften und geerbte Eigenschaften für iOS Store-Apps.

Sie erbt von [mobileApp](../resources/intune_apps_mobileapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[iosStoreApps auflisten](../api/intune_apps_iosstoreapp_list.md)|[iosStoreApp](../resources/intune_apps_iosstoreapp.md)-Sammlung|Listet die Eigenschaften und Beziehungen von Objekten des Typs [iosStoreApp](../resources/intune_apps_iosstoreapp.md) auf.|
|[iosStoreApp abrufen](../api/intune_apps_iosstoreapp_get.md)|[iosStoreApp](../resources/intune_apps_iosstoreapp.md)|Lesen von Eigenschaften und Beziehungen des [iosStoreApp](../resources/intune_apps_iosstoreapp.md)-Objekts.|
|[iosStoreApp erstellen](../api/intune_apps_iosstoreapp_create.md)|[iosStoreApp](../resources/intune_apps_iosstoreapp.md)|Erstellen eines neuen [IosStoreApp](../resources/intune_apps_iosstoreapp.md)-Objekts.|
|[iosStoreApp löschen](../api/intune_apps_iosstoreapp_delete.md)|Keine|Löscht eine [iosStoreApp](../resources/intune_apps_iosstoreapp.md).|
|[iosStoreApp aktualisieren](../api/intune_apps_iosstoreapp_update.md)|[iosStoreApp](../resources/intune_apps_iosstoreapp.md)|Aktualisieren der Eigenschaften eines [iosStoreApp](../resources/intune_apps_iosstoreapp.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Schlüssel der Entität Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|displayName|Zeichenfolge|Der vom Administrator bereitgestellte oder importierte Titel der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|Beschreibung|Zeichenfolge|Beschreibung der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|Verleger|Zeichenfolge|Der Herausgeber der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|isFeatured|Boolesch|Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|privacyInformationUrl|Zeichenfolge|URL zur Datenschutzerklärung. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|informationUrl|Zeichenfolge|URL zur Seite mit weiteren Informationen. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|Besitzer|Zeichenfolge|Der Besitzer der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|Entwickler|Zeichenfolge|Der Entwickler der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|Hinweise|Zeichenfolge|Hinweise zur App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|Der Veröffentlichungsstatus der App. Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.|
|gebündelt|Zeichenfolge|Identitätsname|
|appStoreUrl|Zeichenfolge|URL des Apple-App-Stores|
|applicableDeviceType|[iosDeviceType](../resources/intune_apps_iosdevicetype.md)|Die iOS-Architektur, für die diese App ausgeführt werden kann.|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune_apps_iosminimumoperatingsystem.md)|Der Wert für die Mindestversion des verwendbaren Betriebssystems.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|Kategorien|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Die Liste der Kategorien für diese App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|Aufgaben|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileApp",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosStoreApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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
  "bundleId": "String",
  "appStoreUrl": "String",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```








