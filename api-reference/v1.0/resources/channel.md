# <a name="channel-resource-type"></a>DDE-Kanal Ressourcentyp



Ein Kanal ist eine Auflistung von Nachrichten in einem [Team](../resources/team.md). Ein Kanal stellt ein Thema und daher eine logische Isolierung von Diskussion, innerhalb eines Teams. Beispiele für können DDE-Kanal "Freitag Team Mittagessen" und "Diskussion über Architektur" Channel sein.


## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Liste Kanäle](../api/channel_list.md) | [Kanal](channel.md) -Auflistung | Rufen Sie die Liste der Kanäle in dieser Gruppe.|
|[Erstellen von DDE-Kanal](../api/channel_post.md) | [DDE-Kanal](channel.md) | Erstellen Sie einen neuen Kanal durch das Einbeziehen von den Anzeigenamen und die Beschreibung ein.|
|[Abrufen von DDE-Kanal](../api/channel_get.md) | [DDE-Kanal](channel.md) | Lesen Sie Eigenschaften und Beziehungen des Kanals.|
|[Aktualisieren der DDE-Kanal](../api/channel_patch.md) | [DDE-Kanal](channel.md) | Aktualisieren Sie die Eigenschaften des Kanals.|
|[DDE-Kanal löschen](../api/channel_delete.md) | Keine | Löschen Sie einen Kanal.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|description|Zeichenfolge|Optionale Beschreibung für den Kanal.|
|displayName|Zeichenfolge|Channel-Namen, die dem Benutzer in Microsoft-Teams, erscheint.|
|id|Zeichenfolge|Eindeutiger Bezeichner der Kanäle. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Registerkarten|[TeamsTab](../resources/teamstab.md) -Auflistung|Eine Auflistung aller Registerkarten im Kanal. Eine Navigationseigenschaft.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
