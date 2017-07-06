# <a name="onenoteoperation-resource-type"></a>onenoteOperation-Ressourcentyp

Der Status bestimmter lange dauernder OneNote-Vorgänge.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|createdDateTime| DateTimeOffset |Die Startzeit des Vorgangs.|
|error|[onenoteOperationError](onenoteoperationerror.md)|Der Fehler, der vom Vorgang zurückgegeben wird.|
|id|string|Die Vorgangs-ID. Schreibgeschützt.|
|lastActionDateTime| DateTimeOffset |Der Zeitpunkt der letzten Aktion des Vorgangs.|
|resourceId|string|Die Ressourcen-ID.|
|resourceLocation|string|Der Ressourcen-URI für das Objekt. Beispielsweise der Ressource-URI für eine kopierte Seite oder einen kopierten Abschnitt. |
|status|string|Der aktuellen Status des Vorgangs: `notstarted`, `running`, `completed`, `failed` |
|percentComplete|string|Der abgeschlossene Prozentsatz des Vorgangs, sofern der Vorgang noch den Status `running` hat.

## <a name="relationships"></a>Beziehungen
Keine


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Vorgang abrufen](../api/onenoteoperation_get.md) | [onenoteOperation](onenoteoperation.md) |Dient zum Abrufen des Status des Vorgangs. |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->