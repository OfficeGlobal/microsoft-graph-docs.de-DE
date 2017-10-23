# <a name="workbooksessioninfo-resource-type"></a>workbookSessionInfo-Ressourcentyp

Enthält Informationen zu Arbeitsmappensitzungen.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ  | Beschreibung                               |
|:---------|:------|:------------------------------------------|
| id  | string | Die ID der Arbeitsmappensitzung. |
| persistChanges | string |  `true` für eine beständige Sitzung `false` für eine nicht-beständige Sitzung (Ansichtsmodus) |

