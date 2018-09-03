# <a name="recurrencerange-resource-type"></a>recurrenceRange-Ressourcentyp

Beschreibt den Datumsbereich, über den sich ein wiederkehrendes [Ereignis](event.md) wiederholt. 

Je nach Ihrem Szenario können Sie den Datumsbereich einer Ereignisserie in einer der drei folgenden Arten angeben. Sie müssen zwar immer einen **startDate**-Wert für den Datumsbereich angeben, Sie können aber auch ein wiederkehrendes Ereignis angeben, das an einen angegebenen Datum endet, das nicht endet oder das nach 5 Vorkommen endet. Beachten Sie, dass die tatsächlichen Vorkommen innerhalb des Datumsbereichs immer dem Serienmuster folgen, das Sie für das wiederkehrende Ereignis angeben. Ein wiederkehrendes Ereignis wird immer durch sein [recurrencePattern](recurrencepattern.md) (wie oft sich das Ereignis wiederholt), und seinen **recurrenceRange** (über welche Zeitspanne sich das Ereignis wiederholt) definiert.

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|endDate|Datum|Das Datum zum Beenden des Anwendens des Musters. Je nach dem Serienmuster des Ereignisses ist das letzte Vorkommen der Besprechung möglicherweise nicht an diesem Datum. Erforderlich, wenn **type** `endDate` ist.|
|numberOfOccurrences|Int32|Die Anzahl von Wiederholungen für das Ereignis. Erforderlich; muss positiv sein, wenn **type** `numbered` ist.|
|recurrenceTimeZone|Zeichenfolge |Zeitzone für die **startDate**- und **endDate**-Eigenschaften. Optional. Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet.|
|startDate|Datum|Das Datum zum Starten des Anwendens des Musters. Je nach dem Serienmuster des Ereignisses findet das erste Vorkommen der Besprechung möglicherweise an diesem Datum oder später statt. Muss der gleiche Wert wie die **start**-Eigenschaft des wiederkehrenden [Ereignisses](event.md) sein. Erforderlich.|
|Typ|recurrenceRangeType|Der Serienbereich. Mögliche Werte sind `endDate`, `noEnd` und `numbered`. Erforderlich.|

Verwenden Sie die **Typ**-Eigenschaft, um die unterschiedlichen Typen von **recurrenceRange** anzugeben. Beachten Sie die erforderlichen Eigenschaften für jeden Typ, wie in der folgenden Tabelle beschrieben.

| Typ-Eigenschaft  | Serienbereich-Typ | Beschreibung | Beispiel | Erforderliche Eigenschaften |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |Bereich mit Enddatum | Ereignis an allen Tagen wiederholen, die mit dem entsprechenden Serienmuster zwischen dem **startDate** und dem **endDate** übereinstimmen. | Ereignis im Datumsbereich zwischen 1. Juni 2017 und 15. Juni 2017 wiederholen. | **Typ**, **startDate**, **endDate** | 
|`noEnd`  |Bereich ohne Enddatum | Ereignis an allen Tagen wiederholen, die mit dem entsprechenden Serienmuster beginnend am **startDate** übereinstimmen. | Ereignis im Datumsbereich beginnend am 1. Juni 2017 unbegrenzt wiederholen. | **Typ**, **startDate** |
|`numbered`|Bereich mit einer bestimmten Anzahl von Vorkommen | Ereignis für die **numberOfOccurrences** basierend auf dem Serienmuster beginnend am **startDate** wiederholen. | Ereignis im Datumsbereich beginnend am 1. Juni 2017 für 10 Vorkommen wiederholen.  | **Typ**, **startDate**, **numberOfOccurrences** |


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrenceRange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/resources/recurrencerange.md:
      Failed to parse any rows out of table with headers: | type property  | Type of recurrence range | Description | Example | Required properties |"
  ],
  "tocPath": ""
}-->
