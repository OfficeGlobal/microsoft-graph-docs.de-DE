# <a name="sharepointids-resource-type"></a>SharePointIds-Ressourcentyp

Die **SharePointIds**-Ressource gruppiert die verschiedenen Bezeichner für ein in einer SharePoint-Website oder auf OneDrive for Business gespeichertes Element in einer einzelnen Struktur.

**Hinweis:** von OneDrive Personal zurückgegebene Elemente umfassen kein **SharePointIds**-Facet.

### <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->
```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "webId": "string"
}
```

### <a name="properties"></a>Eigenschaften

| Eigenschaft          | Typ    | Beschreibung                                                          |
|:------------------|:--------|:---------------------------------------------------------------------|
| listId            | string  | Der eindeutige Bezeichner für die Liste des Elements in SharePoint.                          |
| listItemId        | string  | Ein ganzzahliger Bezeichner für das Element innerhalb der Liste.                    |
| listItemUniqueId  | string  | Der eindeutige Bezeichner für das Element in OneDrive for Busienss oder auf einer SharePoint-Website. |
| siteId            | string  | Der eindeutige Bezeichner für die Websitesammlung des Elements. |
| webId             | string  | Der eindeutige Bezeichner für die Websites des Elements.                          |

## <a name="remarks"></a>Bemerkungen 

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharepointIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
