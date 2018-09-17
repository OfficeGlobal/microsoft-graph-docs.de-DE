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
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|Der Veröffentlichungsstatus der App. Eine App kann erst zugewiesen werden, wenn sie veröffentlicht wurde. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md). Mögliche Werte: `notPublished`, `processing` und `published`.|
|appAvailability|[managedAppAvailability](../resources/intune_apps_managedappavailability.md)|Die Verfügbarkeit der Anwendung. Mögliche Werte: `global`, `lineOfBusiness`.|
|Version|Zeichenfolge|Die Version der Anwendung.|

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
  "@odata.type": "microsoft.graph.managedApp"
}-->
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








