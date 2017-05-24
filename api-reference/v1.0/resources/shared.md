# <a name="shared-resource-type"></a>Shared-Ressourcentyp

Die **Shared**-Ressourcenart gibt an, dass ein DriveItem für andere Personen freigegeben wurde. Die Ressource enthält Informationen darüber, wie das Element freigegeben wird.

Wenn ein [**DriveItem**](driveitem.md) ein **shared**-Facet ungleich Null aufweist, wurde das Element freigegeben.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shared",
  "optionalProperties": [ "sharedBy", "sharedDateTime" ]
}-->

```json
{
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "scope": "public | organization | users",
  "sharedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "sharedDateTime": "datetime"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ                          | Beschreibung                                                                                        |
| :------------- | :---------------------------- | :------------------------------------------------------------------------------------------------- |
| owner          | [IdentitySet](identityset.md) | Die Identität der der Besitzer des freigegebenen Elements. Schreibgeschützt.                                           |
| scope          | Zeichenfolge                        | Gibt den Bereich der Freigabe des Elements an: `anonymous`, `organization` oder `users`. Schreibgeschützt. |
| sharedBy       | [identitySet](identityset.md) | Die Identität des Benutzers, der das Element freigegeben hat. Schreibgeschützt.                                           |
| sharedDateTime | DateTimeOffset                | UTC-Datum und -Uhrzeit der Elementfreigabe. Schreibgeschützt.                                         |

## <a name="scope-values"></a>Bereichswerte

| Wert        | Beschreibung                                                                           |
|:-------------|:--------------------------------------------------------------------------------------|
| Öffentlich       | Das Element wird unter Verwendung einer Verknüpfung freigegeben, die für jede Person mit der Link funktioniert.               |
| Organisation | Das Element wird unter Verwendung einer Verknüpfung freigegeben, die für Organisation des Besitzers funktioniert. |
| Benutzer        | Das Element wird nur für bestimmte Benutzern freigegeben.                                          |

## <a name="remarks"></a>Bemerkungen

Weitere Informationen über die Facets einer **driveItem**-Ressource finden Sie unter [**driveItem**](driveitem.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shared resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
