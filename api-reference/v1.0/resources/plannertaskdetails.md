# <a name="plannertaskdetails-resource-type"></a>plannerTaskDetails-Ressourcentyp

Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes [task](plannertask.md)-Objekt hat ein Detailobjekt.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerTaskDetails abrufen](../api/plannertaskdetails_get.md) | [plannerTaskDetails](plannertaskdetails.md) |Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerTaskDetails**-Objekts.|
|[Aktualisieren](../api/plannertaskdetails_update.md) | [plannerTaskDetails](plannertaskdetails.md)    |Dient zum Aktualisieren des **plannerTaskDetails**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Checkliste|[plannerChecklistItems](plannerchecklistitems.md)|Die Sammlung von Checklistenelementen für die Aufgabe.|
|Beschreibung|Zeichenfolge|Beschreibung der Aufgabe.|
|ID|Zeichenfolge| Schreibgeschützt. ID der Aufgabendetails. Sie ist 28 Zeichen lang und berücksichtigt Groß-/Kleinschreibung. Die [Formatvalidierung](planner_identifiers_disclaimer.md) erfolgt für den Dienst.|
|previewType|Zeichenfolge|Hierdurch wird der Typ der Vorschau festgelegt, der für die Aufgabe angezeigt wird. Mögliche Werte sind: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Bei Festlegung auf `automatic` wird die angezeigte Vorschau von der App ausgewählt, die die Aufgabe anzeigt.|
|Verweise|[plannerExternalReferences](plannerexternalreferences.md)|Die Sammlung der Verweise für die Aufgabe.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
