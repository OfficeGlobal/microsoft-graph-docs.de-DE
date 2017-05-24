# <a name="licenseunitsdetail-resource-type"></a>licenseUnitsDetail-Ressourcentyp

Die **prepaidUnits**-Eigenschaft der [subscribedSku](subscribedsku.md)-Entität ist vom Typ **licenseUnitsDetail**.

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:-------------|:-----|:----------|
|aktiviert|Int32| Die Anzahl der Einheiten, die aktiviert werden. |
|suspended|Int32| Die Anzahl der Einheiten, die angehalten werden. |
|warning|Int32| Die Anzahl der Einheiten, für die eine Warnung vorliegt. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
