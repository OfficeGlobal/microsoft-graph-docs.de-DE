# <a name="microsoftstoreforbusinessapp-resource-type"></a>microsoftStoreForBusinessApp-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Microsoft Store für Unternehmen-Apps. Diese Klasse unterstützt keine Methoden zum Erstellen, Aktualisieren oder Löschen.

Sie erbt von [mobileApp](../resources/intune_apps_mobileapp.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[MicrosoftStoreForBusinessApps auflisten](../api/intune_apps_microsoftstoreforbusinessapp_list.md)|[microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)-Objekte.|
|[MicrosoftStoreForBusinessApp abrufen](../api/intune_apps_microsoftstoreforbusinessapp_get.md)|[microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)|Lesen von Eigenschaften und Beziehungen des [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)-Objekts.|
|[MicrosoftStoreForBusinessApp erstellen](../api/intune_apps_microsoftstoreforbusinessapp_create.md)|[microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)|Erstellen eines neuen [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)-Objekts.|
|[MicrosoftStoreForBusinessApp löschen](../api/intune_apps_microsoftstoreforbusinessapp_delete.md)|Keine|Löscht ein [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)-Objekt.|
|[MicrosoftStoreForBusinessApp aktualisieren](../api/intune_apps_microsoftstoreforbusinessapp_update.md)|[microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)|Aktualisieren der Eigenschaften eines [microsoftStoreForBusinessApp](../resources/intune_apps_microsoftstoreforbusinessapp.md)-Objekts.|

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
|usedLicenseCount|Int32|Die Anzahl von verwendeten Microsoft Store für Unternehmen-Lizenzen.|
|totalLicenseCount|Int32|Die Gesamtzahl der Microsoft Store für Unternehmen-Lizenzen.|
|productKey|String|Der Product Key der App|
|licenseType|String|Der Lizenztyp der App. Mögliche Werte: `offline`, `online`.|
|packageIdentityName|String|Bezeichner des App-Pakets|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|Sammlung von Objekten des Typs [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Die Liste der Kategorien für diese App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|
|assignments|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)-Sammlung|Die Liste von Gruppenzuweisungen für diese mobile App. Geerbt von [mobileApp](../resources/intune_apps_mobileapp.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "productKey": "String",
  "licenseType": "String",
  "packageIdentityName": "String"
}
```


