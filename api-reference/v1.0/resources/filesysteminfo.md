# <a name="filesysteminfo-resource-type"></a>Ressourcentyp FileSystemInfo

Die Ressource **FileSystemInfo** enthält Eigenschaften, die vom lokalen Dateisystem des Geräts für die lokale Version eines Elements gemeldet werden. Diese Facet kann zum Angeben des letzten Änderungsdatums oder des Erstellungsdatums des Elements verwendet werden, wie es auf dem lokalen Gerät gespeichert war.

**Hinweis:** Die Eigenschaft **FileSystemInfo** ist nicht für DriveItems in SharePoint oder OneDrive for Business verfügbar.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSystemInfo"
}-->

```json
{
  "createdDateTime": "datetime",
  "lastModifiedDateTime": "datetime"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft                 | Typ           | Beschreibung                                                   |
|:-------------------------|:---------------|:--------------------------------------------------------------|
| **createdDateTime**      | DateTimeOffset | Das UTC-Datum und die UTC-Uhrzeit der Erstellung der Datei auf einem Client.       |
| **lastModifiedDateTime** | DateTimeOffset | Das UTC-Datum und die UTC-Uhrzeit der letzten Änderung der Datei auf einem Client. |

## <a name="notes"></a>Hinweise

Werte für **createdDateTime** und **lastModifiedDateTime** unterscheiden sich von den gleichen Eigenschaften auf der Ressource [DriveItem](driveitem.md). Die Werte für die Ressource DriveItem sind Erstellungsdatum und -uhrzeit, wie sie vom Dienst erfasst werden. Die in der Ressource **FileSystemInfo** gespeicherten Werte werden vom Client bereitgestellt.

Beispiel: Wenn eine Datei am Montag auf dem Gerät erstellt wurde, aber erst am Dienstag in den Dienst hochgeladen wurde, muss der Client, der die Datei hochlädt, die Facet `fileSystemInfo` schreiben, um das Erstellungsdatum am Montag einzubeziehen. Wenn die Metadaten des Elements abgerufen werden, wird als Erstellungsdatum für das Element Dienstag angegeben. Die Facet `fileSystemInfo` zeigt jedoch das ursprüngliche Erstellungsdatum am Montag an.

Diese Eigenschaften sind lese- und schreibgeschützt. Wenn Sie eine Datei hochladen und die lokalen Client-Werte für diese Felder kennen, sollten Sie diese bei der Anfrage einbeziehen.

Wenn der Inhalt der Datei aktualisiert wird und diese Eigenschaften nicht angegeben werden, wird **lastModifiedDateTime** automatisch auf die aktuelle Uhrzeit zurückgesetzt.

## <a name="remarks"></a>Bemerkungen

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSystemInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
