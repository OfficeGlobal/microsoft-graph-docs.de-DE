# <a name="section-resource-type"></a>section-Ressourcentyp

Ein Abschnitt in einem OneNote-Notizbuch. Abschnitte können Seiten enthalten.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|erstellt von|[Identität Set](identityset.md)|Die Identität des Benutzers, des Geräts und der Anwendung, von denen das Element erstellt wurde. Schreibgeschützt.|
|erstelltes Datum und Uhrzeit|Datum Uhrzeit Offset|Das Datum und die Uhrzeit der Erstellung des Abschnitts. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|id|Zeichenfolge|Der eindeutige Bezeichner des Abschnitts.  Schreibgeschützt.|
|ist Standard|Boolesch|Gibt an, ob dies der Standardabschnitt des Benutzers ist. Schreibgeschützt.|
|zuletzt geändert durch|[Identität Set](identityset.md)|Die Identität des Benutzers, des Geräts und der Anwendung, von der das Element erstellt wurde. Schreibgeschützt.|
|zuletzt geänderte Datum und Uhrzeit|Datum Uhrzeit Offset|Das Datum und die Uhrzeit der letzten Änderung des Abschnitts. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.|
|links|[ Abschnitt Links](sectionlinks.md)|Links zum Öffnen des Abschnitts. Der Link `oneNoteClientURL` öffnet den Abschnitt im systemeigenen OneNote-Client, sofern er installiert ist. Der Link `oneNoteWebURL` öffnet den Abschnitt in OneNote Online.|
|Anzeigename|Zeichenfolge|Der Name des Abschnitts. |
|Seiten Url|Zeichenfolge|Der Endpunkt `pages`, an dem Sie Details für alle Seiten im Abschnitt abrufen können. Schreibgeschützt.|
|selbst|Zeichenfolge|Der Endpunkt, an dem Sie Details zum Abschnitt abrufen können. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|seiten|[OnenoteSeite](page.md) Sammlung|Die Sammlung von der Seiten im Abschnitt. Schreibgeschützt. Nullwerte zulassend.|
|Eltern Notizbuch|[Notizbuch](notebook.md)|Das Notizbuch, das den Abschnitt enthält.  Schreibgeschützt.|
|Eltern Abschnittsgruppe|[Abschnittsgruppe](sectiongroup.md)|Die Abschnittsgruppe, die den Abschnitt enthält.  Schreibgeschützt.|

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Get Abschnitt](../api/section_get.md) | [Onenote Abschnitt](section.md) |Dient zum Lesen der Eigenschaften und Beziehungen des Abschnitts.|
|[Seite erstellen](../api/section_post_pages.md) |[Seite](page.md)| Dient zum Erstellen einer Seite durch Veröffentlichung in der pages-Sammlung im angegebenen Abschnitt.|
|[Seiten auflisten](../api/section_list_pages.md) |[Page](page.md)-Sammlung| Dient zum Abrufen einer Sammlung von Seiten im angegebenen Abschnitt.|
|[In Notizbuch kopieren](../api/section_copytonotebook.md)|Keine|Dient zum Kopieren des Abschnitts in ein bestimmtes Notizbuch.|
|[In Abschnittsgruppe kopieren](../api/section_copytosectiongroup.md)|Keine|Dient zum Kopieren des Abschnitts in eine bestimmte Abschnittsgruppe.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
