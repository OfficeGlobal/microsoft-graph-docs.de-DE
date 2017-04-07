# <a name="identityset-resource-type"></a>IdentitySet-Ressourcentyp

Die **IdentitySet**-Ressource ist eine verschlüsselte Sammlung von [identity](identity.md)-Ressourcen. Sie wird verwendet, um eine Reihe von Identitäten darzustellen, die verschiedenen Ereignissen für ein Element zugewiesen sind, z. B. _erstellt von_ oder _zuletzt geändert von_.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "user", "device", "application" ],
  "@odata.type": "microsoft.graph.identitySet"
}-->

```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft    | Typ                    | Beschreibung                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| Anwendung | [Identity](identity.md) | Optional. Die mit dieser Aktion verknüpfte Anwendung. |
| Gerät      | [Identity](identity.md) | Optional. Das mit dieser Konfiguration verknüpfte Gerät.      |
| Benutzer        | [Identity](identity.md) | Optional. Der mit dieser Aktion verknüpfte Benutzer.        |

## <a name="remarks"></a>Bemerkungen 

Informationen zur Verwendung von [IdentitySet](driveitem.md)-Ressourcen finden Sie unter **DriveItem**.


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
