# <a name="mobileapp-resource-type"></a>Ressourcentyp „mobileApp“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine abstrakte Klasse, die grundlegende Eigenschaften von mobilen Intune-Apps enthält
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „mobileApp“](../api/intune_apps_mobileapp_list.md)|Sammlung von Objekten des Typs [mobileApp](../resources/intune_apps_mobileapp.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune_apps_mobileapp.md) auf.|
|[Abrufen von „mobileApp“](../api/intune_apps_mobileapp_get.md)|[mobileApp](../resources/intune_apps_mobileapp.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [mobileApp](../resources/intune_apps_mobileapp.md).|
|[Aktion „assign“](../api/intune_apps_mobileapp_assign.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|displayName|Zeichenfolge|Titel der App (vom Administrator bereitgestellt oder importiert)|
|Beschreibung|Zeichenfolge|Beschreibung der App|
|Herausgeber|Zeichenfolge|Herausgeber der App|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|Das große Symbol, das in den App-Details angezeigt und für den Upload des Symbols verwendet werden soll|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der App|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der App|
|isFeatured|boolesch|Wert, der angibt, ob die App vom Administrator als empfohlen markiert wurde|
|privacyInformationUrl|Zeichenfolge|URL zur Datenschutzerklärung|
|informationUrl|Zeichenfolge|URL zur Seite mit weiteren Informationen|
|Besitzer|Zeichenfolge|Besitzer der App|
|Entwickler|Zeichenfolge|Entwickler der App|
|Notizen|Zeichenfolge|Hinweise zur App|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|Der Status der Veröffentlichung einer App. Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde. Mögliche Werte sind: `notPublished`, `processing`, `published`.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|Kategorien|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Liste der Kategorien, denen die App zugeordnet ist.|
|Aufgaben|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Sammlung|Liste der Gruppenzuweisungen für die mobile App|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
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
  "publishingState": "String"
}
```








