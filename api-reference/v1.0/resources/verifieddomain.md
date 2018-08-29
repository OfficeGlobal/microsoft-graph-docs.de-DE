# <a name="verifieddomain-resource-type"></a>verifiedDomain-Ressourcentyp

Gibt eine Domäne für einen Mandanten an. Die **verifiedDomains**-Eigenschaft der [organization](organization.md)-Entität ist eine Auflistung von **VerifiedDomain**.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Funktionen|String|Zum Beispiel „Email“, „OfficeCommunicationsOnline“.|
|isDefault|Boolean|                **true**, wenn dies die Standarddomäne ist, die dem Mandanten zugeordnet ist, andernfalls **false**.            |
|isInitial|Boolean|**true**, wenn dies die ursprüngliche Domäne ist, die dem Mandanten zugeordnet ist, andernfalls **false**.|
|name|String|Der Domänenname, zum Beispiel „contoso.onmicrosoft.com“|
|type|String|Z. B. „verwaltet“.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedDomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
