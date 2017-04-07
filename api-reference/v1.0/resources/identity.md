# <a name="identity-resource-type"></a>identity-Ressourcentyp

Die **Identity**-Ressource stellt eine Identität von einem _Akteur_ dar. Ein Akteur kann z. B. ein Benutzer, Gerät oder eine Anwendung sein.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft    | Typ   | Beschreibung                                                                                                                                                                                                                                                                                                           |
|:------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| displayName | String | Der Anzeigenamen der Identität. Beachten Sie, dass dieser möglicherweise nicht immer verfügbar oder auf dem neuesten Stand ist. Wenn sich z. B. der Anzeigename eines Benutzers ändert, zeigt die API möglicherweise den neuen Wert in einer zukünftigen Antwort an, aber für die dem Benutzer zugeordneten Elemente wird mit [Änderungen suchen](../api/item_delta.md) nicht angezeigt, dass sie sich geändert haben. |
| id          | String | Eindeutiger Bezeichner für die Identität.                                                                                                                                                                                                                                                                                   |

## <a name="remarks"></a>Bemerkungen

Unter gewissen Umständen steht der eindeutige Bezeichner für den Akteur möglicherweise nicht zur Verfügung. In diesem Fall die wird die Eigenschaft **DisplayName** für die Identität zurückgegeben werden, aber die **Id**-Eigenschaft ist aus der Ressource nicht vorhanden.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
