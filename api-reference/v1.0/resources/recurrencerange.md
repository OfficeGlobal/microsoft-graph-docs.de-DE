# <a name="recurrencerange-resource-type"></a>recurrenceRange-Ressourcentyp

Beschreibt den Datumsbereich, über den sich ein wiederkehrendes [Ereignis](event.md) wiederholt. 

Je nach Ihrem Szenario können Sie den Datumsbereich einer Ereignisserie in einer der drei folgenden Arten angeben. Sie müssen zwar immer einen **startDate**-Wert für den Datumsbereich angeben, Sie können aber beispielsweise ein wiederkehrendes Ereignis angeben, das an einen angegebenen Datum endet, das nicht endet oder das nach 5 Vorkommen endet. Beachten Sie, dass die tatsächlichen Vorkommen innerhalb des Datumsbereichs immer dem Serienmuster folgen, das Sie für das wiederkehrende Ereignis angeben. Ein wiederkehrendes Ereignis wird immer durch sein [recurrencePattern](recurrencepattern.md) (wie oft sich das Ereignis wiederholt), und seinen **recurrenceRange** (über welchen Zeitraum sich das Ereignis wiederholt) definiert.

Verwenden Sie die **type**-Eigenschaft, um die unterschiedlichen Typen von **recurrenceRange** anzugeben. Beachten Sie die erforderlichen Eigenschaften für jeden Typ, wie in der folgenden Tabelle beschrieben.

| Typ des Serienbereichs | Wert der type-Eigenschaft | Beschreibung | Beispiel | Erforderliche Eigenschaften |
|:---------------|:--------|:--------|:--------|:----------|
|Bereich mit Enddatum | `endDate` | Ereignis an allen Tagen wiederholen, die mit dem entsprechenden Serienmuster zwischen dem **startDate** und dem **endDate** übereinstimmen. | Ereignis im Datumsbereich zwischen 1. Juni 2017 und 15. Juni 2017 wiederholen. | **type**, **startDate**, **endDate** | 
|Bereich ohne Enddatum | `noEnd` | Ereignis an allen Tagen wiederholen, die mit dem entsprechenden Serienmuster beginnend am **startDate** übereinstimmen. | Ereignis im Datumsbereich beginnend am 1. Juni 2017 unbegrenzt wiederholen. | **type**, **startDate** |
|Bereich mit einer bestimmten Anzahl von Vorkommen | `numbered` | Ereignis für die **numberOfOccurrences** basierend auf dem Serienmuster beginnend am **startDate** wiederholen. | Ereignis im Datumsbereich beginnend am 1. Juni 2017 für 10 Vorkommen wiederholen.  | **type**, **startDate**, **numberOfOccurrences** |


## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|endDate|Datum|Das Datum zum Beenden des Anwendens des Musters. Je nach dem Serienmuster des Ereignisses ist das letzte Vorkommen der Besprechung möglicherweise nicht an diesem Datum. Erforderlich, wenn **type** `endDate` ist.|
|numberOfOccurrences|Int32|Die Anzahl von Wiederholungen für das Ereignis. Erforderlich; muss positiv sein, wenn **type** `numbered` ist.|
|recurrenceTimeZone|String |Zeitzone für die **startDate**- und **endDate**-Eigenschaften. Optional. Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet.|
|startDate|Datum|Das Datum zum Starten des Anwendens des Musters. Je nach dem Serienmuster des Ereignisses findet das erste Vorkommen der Besprechung möglicherweise an diesem Datum oder später statt. Muss der gleiche Wert wie die **start**-Eigenschaft des wiederkehrenden [Ereignisses](event.md) sein. Erforderlich.|
|type|Zeichenfolge|Der Serienbereich. Mögliche Werte: `endDate`, `noEnd`, `numbered`. Erforderlich.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencerange"
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
  "tocPath": ""
}-->
