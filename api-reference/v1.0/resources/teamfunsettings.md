# <a name="teamfunsettings-resource-type"></a>Ressourcentyp teamFunSettings



Einstellungen zum Konfigurieren der Verwendung von Giphy, Memes und Aufkleber in das [Team](team.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowGiphy|Boolescher Wert|Wenn auf "true" ermöglicht Giphy Verwendung festgelegt.|
|giphyContentRating|Zeichenfolge (Aufzählung)|Giphy bewerten. Mögliche Werte sind: `moderate` und `strict`.|
|allowStickersAndMemes|Boolescher Wert|Wenn Festlegung auf "true" ermöglicht Benutzern das Aufkleber und Memes enthalten.|
|allowCustomMemes|Boolescher Wert|Wenn auf "true" ermöglicht Benutzern das Einschließen von benutzerdefinierten Memes festgelegt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
