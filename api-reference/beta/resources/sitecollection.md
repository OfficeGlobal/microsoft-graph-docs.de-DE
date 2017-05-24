# <a name="sitecollection-resource"></a>SiteCollection-Ressource

Die **siteCollection**-Ressource stellt weitere Informationen zu einer Websitesammlung bereit.

Wenn eine [ **site** ](site.md)-Ressource eine **siteCollection**-Eigenschaft mit einem Wert ungleich NULL hat, ist die Website eine Stammwebsite einer Websitesammlung.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname | Typ    | Beschreibung                                                                                                                  |
|:--------------|:--------|:---------------------------------------------------
| **hostname**  | string  | Der Hostname der Websitesammlung. Schreibgeschützt.


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
