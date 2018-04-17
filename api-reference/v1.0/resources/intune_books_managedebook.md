# <a name="managedebook-resource-type"></a>managedEBook-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedEBooks auflisten](../api/intune_books_managedebook_list.md)|[managedEBook](../resources/intune_books_managedebook.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedEBook](../resources/intune_books_managedebook.md)-Objekte.|
|[managedEBook abrufen](../api/intune_books_managedebook_get.md)|[managedEBook](../resources/intune_books_managedebook.md)|Lesen von Eigenschaften und Beziehungen des [managedEBook](../resources/intune_books_managedebook.md)-Objekts.|
|[Aktion zuweisen](../api/intune_books_managedebook_assign.md)|Keine|Noch nicht dokumentiert.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|displayName|String|Name des E-Books|
|description|String|Beschreibung|
|publisher|String|Herausgeber|
|publishedDateTime|DateTimeOffset|Datum und Uhrzeit der Veröffentlichung des E-Books.|
|largeCover|[mimeContent](../resources/intune_books_mimecontent.md)|Umschlagbild des Buchs|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der E-Book-Datei.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des E-Books.|
|informationUrl|String|URL zur Seite mit weiteren Informationen.|
|privacyInformationUrl|String|URL zur Datenschutzerklärung|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[managedEBookAssignment](../resources/intune_books_managedebookassignment.md)-Sammlung|Die Liste der Zuweisungen für dieses E-Book.|
|installSummary|[eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md)|Die Installationszusammenfassung für die mobile App.|
|deviceStates|[deviceInstallState](../resources/intune_books_deviceinstallstate.md)-Sammlung|Die Liste der Installationsstatus für das E-Book.|
|userStateSummary|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)-Sammlung|Die Liste der Installationsstatus für das E-Book.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
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
  "privacyInformationUrl": "String"
}
```



