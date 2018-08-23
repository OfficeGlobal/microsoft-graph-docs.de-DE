# <a name="operation-resource-type"></a>Vorgangs-Ressourcentyp

Der Status eines zeitintensiven Vorgangs.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|createdDateTime| DateTimeOffset |Die Startzeit des Vorgangs.|
|lastActionDateTime| DateTimeOffset |Der Zeitpunkt der letzten Aktion des Vorgangs.|
|Status|operationStatus|Der aktuellen Status des Vorgangs: `notStarted`, `running`, `completed`, `failed` |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
