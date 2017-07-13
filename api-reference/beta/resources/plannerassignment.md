# plannerAssignment-Ressourcentyp
<a id="plannerassignment-resource-type" class="xliff"></a>

Die **plannerAssignment**-Ressource stellt die Zuweisung einer Aufgabe zu einem Benutzer dar. Dieser Typ wird im offenen Typ [plannerAssignments](plannerassignments.md) verwendet.


## Eigenschaften
<a id="properties" class="xliff"></a>
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|assignedBy|[identitySet](identityset.md)|Die Identität des Benutzers, der die Zuweisung der Aufgabe durchgeführt hat, d. h. der Zuweisende.|
|assignedDateTime|DateTimeOffset|Uhrzeit, zu der die Aufgabe zugewiesen wurde. Der Zeitstempeltyp stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|orderHint|String|Hinweis, der verwendet wird, um zugewiesene Personen in einer Aufgabe anzuordnen. Das Format ist wie [hier](planner_order_hint_format.md) beschrieben definiert.|

## JSON-Darstellung
<a id="json-representation" class="xliff"></a>
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignment"
}-->

```json
{
  "assignedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "assignedDateTime": "String (timestamp)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->