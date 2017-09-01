# <a name="itemreference-resource-type"></a>ItemReference-Ressourcentyp

Die **ItemReference**-Ressource enthält Informationen, die erforderlich sind, um ein [DriveItem](driveitem.md) über die API zu adressieren.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft      | Typ                              | Beschreibung                                                                                                |
| :------------ | :-------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| driveId       | Zeichenfolge                            | Eindeutiger Bezeichner der drive-Instanz, die das Element enthält. Schreibgeschützt.                                 |
| id            | String                            | Eindeutiger Bezeichner des Elements im Laufwerk. Schreibgeschützt.                                                     |
| name          | Zeichenfolge                            | Der Name des Elements, auf das verwiesen wird. Schreibgeschützt.                                                          |
| Pfad          | String                            | Pfad, der verwendet werden kann, um zu dem Element zu navigieren. Schreibgeschützt.                                                  |
| shareId       | String                            | Ein eindeutiger Bezeichner für eine freigegebene Ressource, auf die über [Freigabe](../api/shares_get.md)-API zugegriffen werden kann. |
| sharepointIds | [sharepointIds](sharepointids.md) | Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.                                   |

## <a name="remarks"></a>HinwBemerkungeneise

Um ein **driveItem**-Element aus einer **itemReference**-Ressource zu adressieren, erstellen Sie eine URL im folgenden Format:

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

Der **path**-Wert ist ein API-Pfad relativ zu dem Ziellaufwerk, z. B.: `/drive/root:/Documents/myfile.docx`.

Um den lesbaren Pfad für ein Breadcrumb abzurufen, können Sie alles bis zum ersten `:` in der Pfadzeichenfolge problemlos ignorieren.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
