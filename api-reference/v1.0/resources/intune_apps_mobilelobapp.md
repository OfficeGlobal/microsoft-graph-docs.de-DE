# <a name="mobilelobapp-resource-type"></a>mobileLobApp-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine abstrakte Basisklasse mit Eigenschaften für alle mobilen branchenspezifischen Apps.

Sie erbt von [mobileApp](../resources/intune_apps_mobileapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[MobileLobApps auflisten](../api/intune_apps_mobilelobapp_list.md)|[mobileLobApp](../resources/intune_apps_mobilelobapp.md)-Sammlung|Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileLobApp](../resources/intune_apps_mobilelobapp.md) auf.|
|[MobileLobApp abrufen](../api/intune_apps_mobilelobapp_get.md)|[mobileLobApp](../resources/intune_apps_mobilelobapp.md)|Liest die Eigenschaften und Beziehungen von Objekten des [mobileLobApp](../resources/intune_apps_mobilelobapp.md)-Objekts auf.|

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
|committedContentVersion|String|Die interne zugesicherte Inhaltsversion.|
|fileName|String|Der Name der Hauptdatei der Branchenanwendung.|
|size|Int64|Die Gesamtgröße einschließlich aller hochgeladenen Dateien.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Die Liste der Kategorien für diese App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|assignments|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|contentVersions|Sammlung von Objekten des Typs [mobileAppContent](../resources/intune_apps_mobileappcontent.md)|Die Liste der Inhaltsversionen für diese App.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileLobApp",
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
  "size": 1024
}
```



