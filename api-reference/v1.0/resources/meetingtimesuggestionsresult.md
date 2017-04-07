# <a name="meetingtimesuggestionsresult-resource-type"></a>Ressourcentyp „meetingTimeSuggestionsResult“

Dieser Ressourcentyp listet eine Sammlung von Besprechungsvorschlägen auf, sofern Vorschläge zurückgegeben werden, oder den Grund, aus dem keine Vorschläge zurückgegeben werden.

In der folgenden Tabelle finden Sie mögliche Gründe, aus denen [findMeetingTimes](../api/user_findmeetingtimes.md) keine Besprechungsvorschläge zurückgibt.

|**Wert für „emptySuggestionsReason“**|**Gründe**|
|:-----|:-----|
| attendeesUnavailable | Die Verfügbarkeit jedes Teilnehmers ist bekannt, die Zahl der verfügbaren Teilnehmer liegt jedoch für jedes Zeitfenster unter dem Konfidenzschwellenwert für die Besprechung. Dieser ist standardmäßig auf 50 % gesetzt. Basis für den Schwellenwert ist der Frei-/Gebucht-Status der einzelnen Teilnehmer für ein vorgeschlagenes Besprechungszeitfenster. Dabei entspricht der Status „Frei“ einer Teilnahmewahrscheinlichkeit von 100 %, der Status „Unbekannt“ einer Teilnahmewahrscheinlichkeit von 49 % und der Status „Gebucht“ einer Teilnahmewahrscheinlichkeit von 0 %.|
| attendeesUnavailableOrUnknown | Die Verfügbarkeit einiger oder aller Teilnehmer ist unbekannt, sodass die Besprechungskonfidenz unter dem definierten Schwellenwert liegt. Dieser ist standardmäßig auf 50 % gesetzt. Die Verfügbarkeit eines Teilnehmers kann unbekannt sein, wenn der Teilnehmer nicht zur Organisation gehört oder ein Fehler beim Abruf der Frei-/Gebucht-Informationen auftritt.|
| locationsUnavailable | Die Eigenschaft **isRequired** des Parameters [locationConstraint](locationconstraint.md) ist als obligatorisch festgelegt, aber es sind während der berechneten Zeitfenster keine Orte verfügbar. |
| organizerUnavailable | Der Parameter **isOrganizerOptional** ist auf „false“ gesetzt, der Organisator ist aber während des angefragten Zeitfensters nicht verfügbar. |
| unknown | Der Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden, ist nicht bekannt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult"
}-->

```json
{
  "emptySuggestionsReason": "String",
  "meetingTimeSuggestions": [{"@odata.type": "microsoft.graph.meetingTimeSuggestion"}]
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|emptySuggestionsReason|Zeichenfolge|Ein Grund, aus dem keine Besprechungsvorschläge zurückgegeben wurden. Mögliche Werte sind: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` und `unknown`.|
|meetingTimeSuggestions|[meetingTimeSuggestion](meetingTimeSuggestion.md) collection|Ein Array von Besprechungsvorschlägen|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->