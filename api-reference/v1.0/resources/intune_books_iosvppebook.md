# <a name="iosvppebook-resource-type"></a>Ressourcentyp „iosVppEBook“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Klasse enthält die Eigenschaften eines iOS-VPP-E-Books.

Sie erbt von [managedEBook](../resources/intune_books_managedebook.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „iosVppEBook“](../api/intune_books_iosvppebook_list.md)|Sammlung von Objekten des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md) auf.|
|[Abrufen von „iosVppEBook“](../api/intune_books_iosvppebook_get.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md).|
|[Erstellen von „iosVppEBook“](../api/intune_books_iosvppebook_create.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md)|Erstellt neue Objekte des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md).|
|[Löschen von „iosVppEBook“](../api/intune_books_iosvppebook_delete.md)|Keiner|Löscht Objekte des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md).|
|[Aktualisieren von „iosVppEBook“](../api/intune_books_iosvppebook_update.md)|[iosVppEBook](../resources/intune_books_iosvppebook.md)|Aktualisiert die Eigenschaften von Objekten des Typs [iosVppEBook](../resources/intune_books_iosvppebook.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Der Schlüssel der Entität. Der Wert wird geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|displayName|String|Der Name des E-Books. Der Wert wird geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|description|String|Beschreibung. Der Wert wird geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|publisher|String|Herausgeber. Der Wert wird geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|publishedDateTime|DateTimeOffset|Datum und Uhrzeit der Veröffentlichung des E-Books. Der Wert wird geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|largeCover|[mimeContent](../resources/intune_books_mimecontent.md)|Umschlagbild des Buchs. Der Wert wird geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der E-Book-Datei. Der Wert wird geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des E-Books. Der Wert wird geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|informationUrl|String|URL zur Seite mit weiteren Informationen. Der Wert wird geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|privacyInformationUrl|String|URL zur Datenschutzerklärung. Der Wert wird geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|vppTokenId|Guid|ID des VPP-Tokens|
|appleId|String|Apple-ID, die dem VPP-Token zugeordnet ist|
|vppOrganizationName|String|Zum VPP-Token gehörender Organisationsname|
|genres|String-Sammlung|Genres|
|language|String|Sprache|
|seller|String|Verkäufer|
|totalLicenseCount|Int32|Gesamtanzahl von Lizenzen|
|usedLicenseCount|Int32|Gesamtanzahl von genutzten Lizenzen|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|Sammlung von Objekten des Typs [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)|Die Liste der Zuweisungen des E-Books. Der Wert wird geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|installSummary|[eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md)|Die Installationszusammenfassung für die mobile App. Der Wert wird geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|deviceStates|Sammlung von Objekten des Typs [deviceInstallState](../resources/intune_books_deviceinstallstate.md)|Die Liste der Installationsstatus für das E-Book. Der Wert wird geerbt von [managedEBook](../resources/intune_books_managedebook.md).|
|userStateSummary|Sammlung von Objekten des Typs [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|Die Liste der Installationsstatus für das E-Book. Der Wert wird geerbt von [managedEBook](../resources/intune_books_managedebook.md).|

## <a name="json-representation"></a>JSON-Darstellung
Unten sehen Sie eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String",
  "vppTokenId": "<Unknown Primitive Type Edm.Guid>",
  "appleId": "String",
  "vppOrganizationName": "String",
  "genres": [
    "String"
  ],
  "language": "String",
  "seller": "String",
  "totalLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```



