# <a name="shareddriveitem-resource-type"></a>sharedDriveItem-Ressourcentyp

Die **sharedDriveItem**-Ressource wird zurückgegeben, wenn die [Freigabe](../api/shares_get.md)-API für den Zugriff auf ein freigegebenes[driveItem](driveitem.md)-Objekt verwendet wird.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **sharedDriveItem**-Ressource.

Die **sharedDriveItem**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.

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

    /* relationships*/
    "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
    "root": { "@odata.type": "microsoft.graph.driveItem" },
    "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
    "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ                          | Beschreibung                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| id       | String                        | Die eindeutige ID der Freigabe, auf die zugegriffen wird.              |
| name     | String                        | Der Anzeigename für das freigegebene Element.                             |
| owner    | [IdentitySet](identityset.md) | Informationen zum Besitzer des freigegebenen Elements, auf das verwiesen wird. |

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ                                  | Beschreibung                                                                                                                                                                                                |
| :----------- | :------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Elemente        | Sammlung ([driveItem](driveitem.md)) | Eine Sammlung von freigegebenen **driveItem**-Ressourcen. Diese Sammlung kann nicht aufgezählt werden, aber es kann über die eindeutige ID auf Elemente zugegriffen werden.                                                                        |
| root         | [DriveItem](driveitem.md)             | Das freigegebene **driveItem**-Objekt der obersten Ebene. Wenn eine einzelne Datei freigegeben ist, ist dieses Element die Datei. Wird ein Ordner freigegeben, ist das Element der Ordner. Mit den Facets des Elements können Sie bestimmen, welcher Fall gilt. |
| driveItem    | [driveItem](driveitem.md)             | Eine **driveItem**-Objekt für die Ressource, die freigegeben wurde.  Dies ist identisch mit der **root**-Eigenschaft.                                                                                                             |
| site         | [site](site.md)                       | Eine **site**-Ressource, die das freigegebene Element enthält.                                                                                                                                                |

## <a name="methods"></a>Methoden

| Method                                  | REST-Pfad                |
| :-------------------------------------- | :----------------------- |
| [Freigegebenes Element abrufen](../api/shares_get.md) | `GET /shares/{share-id}` |

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