# <a name="shareddriveitem-resource-type"></a>Ressourcenart SharedDriveItem

Die **SharedDriveItem** Ressource wird zurückgegeben, wenn die [Freigabe](../api/shares_get.md)API für den Zugriff auf [DriveItem](driveitem.md) verwendet wird. Diese Ressource ist vergleichbar mit einer [Laufwerk](drive.md)-Ressource, ist jeoch auf die DriveItems beschränkt, auf die über den Freigabe-Link oder die ShareId zugegriffen werden kann.

### <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->
```json
{
    "id": "string",
    "name": "string",
    "owner": { "@odata.type": "microsoft.graph.identitySet" },
    "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
    "root": { "@odata.type": "microsoft.graph.driveItem" }
}
```

### <a name="properties"></a>Eigenschaften

| Eigenschaft  | Typ                                  | Beschreibung                                                          |
|:----------|:--------------------------------------|:---------------------------------------------------------------------|
| id        | String                                | Die eindeutige ID der Freigabe, auf die zugegriffen wird.                  |
| name      | String                                | Der Anzeigename für das freigegebene Element.                                 |
| owner     | [IdentitySet](identityset.md)         | Informationen zum Besitzer des freigegebenen Elements, auf das verwiesen wird.     |
| items     | Collection([DriveItem](driveitem.md)) | Eine Zusammenstellung von freigegebenen DriveItem-Ressourcen. Diese Zusammenstellung kann nicht aufgelistet werden, aber es kann über die eindeutige ID auf Elemente zugegriffen werden. |
| root      | [DriveItem](driveitem.md)             | Das oberste freigegebene DriveItem. Wenn eine einzelne Datei freigegeben ist, ist dieses Element die Datei. Wird ein Ordner freigegeben, ist das Element der Ordner. Mit den Facets des Elements können Sie bestimmen, welcher Fall gilt. |

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