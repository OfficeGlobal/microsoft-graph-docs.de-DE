# <a name="onpremisesextensionattributes-resource-type"></a>Ressourcentyp onPremisesExtensionAttributes

Die Eigenschaft **onPremisesExtensionAttribute** der [Benutzer](user.md)-Entität enthält fünfzehn benutzerdefinierte Erweiterungsattributseigenschaften. Für einen **onPremisesSyncEnabled**-Benutzer wird diese Eigenschaftengruppe auf dem lokalen Active Directory gemastert und mit Azure AD synchronisiert. Sie ist schreibgeschützt. Für einen Nur-Cloud-Benutzer (wobei **onPremisesSyncEnabled** falsch ist) können diese Eigenschaften während der Erstellung oder der Aktualisierung festgelegt werden.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|extensionAttribute1|Zeichenfolge| Erste anpassbares Erweiterungsattribut. |
|extensionAttribute2|Zeichenfolge| Zweites anpassbares Erweiterungsattribut. |
|extensionAttribute3|Zeichenfolge| Drittes anpassbares Erweiterungsattribut. |
|extensionAttribute4|Zeichenfolge| Viertes anpassbares Erweiterungsattribut. |
|extensionAttribute5|Zeichenfolge| Fünftes anpassbares Erweiterungsattribut. |
|extensionAttribute6|Zeichenfolge| Sechstes anpassbares Erweiterungsattribut. |
|extensionAttribute7|Zeichenfolge| Siebtes anpassbares Erweiterungsattribut. |
|extensionAttribute8|Zeichenfolge| Achtes anpassbares Erweiterungsattribut. |
|extensionAttribute9|Zeichenfolge| Neuntes anpassbares Erweiterungsattribut. |
|extensionAttribute10|Zeichenfolge| Zehntes anpassbares Erweierungsattribut. |
|extensionAttribute11|Zeichenfolge| Elftes anpassbares Erweiterungsattribut. |
|extensionAttribute12|Zeichenfolge| Zwölftes anpassbares Erweiterungsattribut. |
|extensionAttribute13|Zeichenfolge| Dreizehntes anpassbares Erweiterungsattribut. |
|extensionAttribute14|Zeichenfolge| Vierzehntes anpassbares Erweiterungsattribut. |
|extensionAttribute15|Zeichenfolge| Fünfzehntes anpassbares Erweiterungsattribut. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->