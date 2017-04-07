# <a name="timeconstraint-resource-type"></a>Ressourcentyp „timeConstraint“

Die Zeitfenster, in denen eine Aktivität der angegebenen Art stattfinden darf

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeconstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|activityDomain|String|Die Art der Aktivität. Diese Angabe ist optional. Mögliche Werte sind: `unknown`, `work` und `personal`. Aktuell geht [findMeetingTimes](../api/user_findmeetingtimes.md) grundsätzlich vom Wert `work` aus und gibt nur Besprechungsvorschläge innerhalb der Arbeitszeiten des Organisators oder Teilnehmers zurück.|
|timeslots|[timeSlot](timeslot.md) collection|Ein Array von Zeitfenstern|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->