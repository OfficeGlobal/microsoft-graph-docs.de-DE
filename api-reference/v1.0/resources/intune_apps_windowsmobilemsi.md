# <a name="windowsmobilemsi-resource-type"></a>Ressourcentyp „windowsMobileMSI“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Ressource enthält die Eigenschaften und geerbten Eigenschaften einer branchenspezifischen Windows Mobile-MSI-App.

Sie erbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „windowsMobileMSI“](../api/intune_apps_windowsmobilemsi_list.md)|Sammlung von Objekten des Typs [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) auf.|
|[Abrufen von „windowsMobileMSI“](../api/intune_apps_windowsmobilemsi_get.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).|
|[Erstellen von „windowsMobileMSI“](../api/intune_apps_windowsmobilemsi_create.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)|Erstellt neue Objekte des Typs [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).|
|[Löschen von „windowsMobileMSI“](../api/intune_apps_windowsmobilemsi_delete.md)|Keiner|Löscht Objekte des Typs [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).|
|[Aktualisieren von „windowsMobileMSI“](../api/intune_apps_windowsmobilemsi_update.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)|Aktualisiert die Eigenschaften von Objekten des Typs [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|displayName|String|Der vom Administrator bereitgestellte oder importierte Titel der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|description|String|Beschreibung der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|publisher|String|Der Herausgeber der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|isFeatured|Boolean|Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|privacyInformationUrl|String|URL zur Datenschutzerklärung. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|informationUrl|String|URL zur Seite mit weiteren Informationen. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|owner|String|Der Besitzer der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|developer|String|Der Entwickler der App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|notes|String|Hinweise zur App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|Der Veröffentlichungsstatus der App. Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde. Geerbt von [MobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte sind: `notPublished`, `processing` und `published`.|
|committedContentVersion|Zeichenfolge|Die interne zugesicherte Inhaltsversion. Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|
|fileName|Zeichenfolge|Name der Hauptdatei der Branchenanwendung. Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|
|size|Int64|Gesamtgröße einschließlich aller hochgeladenen Dateien. Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|
|commandLine|Zeichenfolge|Befehlszeile|
|productCode|Zeichenfolge|Produktcode|
|productVersion|Zeichenfolge|Produktversion der branchenspezifischen Windows Mobile-MSI-App.|
|ignoreVersionDetection|Boolescher Wert|Boolescher Wert, der steuert, ob nach der Installation der App auf einem Gerät die App-Version zur Erkennung der App verwendet werden soll. Setzen Sie diese Eigenschaft auf „true“ bei branchenspezifischen Windows Mobile-MSI-Apps, die sich selbstständig aktualisieren.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Die Liste der Kategorien für diese App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|assignments|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|contentVersions|Sammlung von Objekten des Typs [mobileAppContent](../resources/intune_apps_mobileappcontent.md)|Liste der Versionen der App-Inhalte. Geerbt von [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsMobileMSI"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "String",
  "productCode": "String",
  "productVersion": "String",
  "ignoreVersionDetection": true
}
```



