# <a name="historyitem-resource-type"></a>Ressourcentyp historyItem

Stellt ein Historienelement für eine [ Aktivität](projectrome_activity.md) in einer App dar. Benutzeraktivitäten stellen ein einziges Ziel in der App dar, beispielsweise ein TV-Programm, ein Dokument oder eine aktuelle Kampagne in einem Videospiel. Wenn ein Benutzer diese Aktivität einbezieht, wird das Engagement als Element des Ereignisprotokolls erfasst, das die Start- und Endzeit für diese Aktivität angibt. Wenn der Benutzer diese Aktivität im Laufe der Zeit erneut einbezieht, werden mehrere Elemente des Ereignisprotokolls als eine einzelne Benutzeraktivität aufgezeichnet.

Wenn von einer Anwendung eine Sitzung erstellt wird, sollte ein **Historienelement** zum **Aktivität** -Objekt entsprechend dem Zeitraum eines Auftrags für Benutzer hinzugefügt werden. Sobald ein Benutzer eine Aktivität wieder aufnimmt, wird der Aktivität ein neues **Historienelement** hinzugefügt, um das Benutzerengagement weiter ansteigen zu lassen.

## <a name="methods"></a>Methoden

|Methode | Rückgabetyp | Beschreibung|
|:------|:------------|:-----------|
|[Erstellen oder Ersetzen eines Historienelements](../api/projectrome_put_historyitem.md) | [historyItem](projectrome_historyitem.md) | Erstellt oder ersetzt ein vorhandenes **Historienelement** für diese Aktivität (Upsert). Die ID muss eine GUID sein.|
|[Löschen eines Historienelements](../api/projectrome_delete_historyitem.md) | Kein Inhalt | Löscht das angegebene **Historienelement** für diese Aktivität.|

## <a name="properties"></a>Eigenschaften

|Name | Typ | Beschreibung|
|:----|:-----|:-----------|
|status | status | Vom Server festgelegt. Ein Statuscode, der dazu verwendet wird, um gültige Objekte identifizieren. Werte: aktiv, aktualisiert, gelöscht, ignoriert.|
|Benutzer Zeitzone | Zeichenfolge | Optional. Die Zeitzone, in der das Gerät des Benutzers zum Zeitpunkt der Erstellung der Aktivität verwendet wurde. Werte, die zur Unterstützung der plattformübergreifenden Darstellung als Olson-IDs angegeben werden.|
|createdDateTime | DateTimeOffset | Vom Server festgelegt. DateTime in UTC, als das Objekt auf dem Server erstellt wurde.|
|lastModifiedDateTime | DateTimeOffset | Vom Server festgelegt. DateTime in UTC, als das Objekt auf dem Server geändert wurde.|
|id | Zeichenfolge | Erforderlich. Vom Client festgelegte GUID für das **historyItem** -Objekt.|
|startedDateTime | DateTimeOffset | Erforderlich. UTC-DateTime zum Beginn des**historyItem** (Aktivitätssitzung). Erforderlich für den Timeline-Verlauf.|
|lastActiveDateTime | DateTimeOffset | Optional. UTC-DateTime beim letzten mal, als **Historienelement** (Aktivitätssitzung) als aktiv oder fertig verstanden wurden - bei null sollte der**Historienelement** Status laufend sein.|
|expirationDateTime | DateTimeOffset | Optional. UTC-DateTime, wenn das **Historienelement** endgültig gelöscht wird. Kann vom Client festgelegt werden.|
|activeDurationSeconds | int | Optional. Die Dauer des Engagements aktiver Benutzer. Wenn nichts angegeben wurde, erfolgt die Berechnung durch **StartedDateTime** und **LastActiveDateTime**.|

## <a name="relationships"></a>Beziehungen

|Beziehung | Typ | Beschreibung|
|:------------|:-----|:-----------|
|activity| [userActivity](../resources/projectrome_activity.md) | Optional. NavigationProperty/Kapselung; Navigationseigenschaft der zugeordneten Aktivität.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
    "status": "active | updated | deleted | ignored",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
