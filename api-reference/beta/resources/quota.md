# <a name="quota-resource-type"></a>quota-Ressourcentyp

Die **quota**-Ressource enthält Details zu Leerzeichenbeschränkungen auf einer[Laufwerk](drive.md)-Ressource.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname | Typ   | Beschreibung                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| gesamt         | Int64  | Zulässige Speicherplatz in Byte. Schreibgeschützt.                           |
| verwendet          | Int64  | Gesamter verwendeter Speicherplatz in Byte. Schreibgeschützt.                                      |
| verbleibende     | Int64  | Gesamter verbleibender Speicherplatz vor dem Erreichen des Speicherkontingents in Byte. Schreibgeschützt. |
| gelöscht       | Int64  | Gesamte Dateien genutzter Speicherplatz im Papierkorb in Byte. Schreibgeschützt.      |
| state         | string | Wert der Enumeration, die den Zustand des Speicherplatzes angibt. Schreibgeschützt. |

## <a name="state-enumeration"></a>Status Enumeration

| Wert      | Beschreibung                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | Das Laufwerk verfügt über ausreichend verbleibendes Kontingent.                                                                                                                               |
| `nearing`  | Verbleibendes Kontingent weniger als 10 % des gesamten Kontingentplatzes.                                                                                                                      |
| `critical` | Verbleibendes Kontingent weniger als 1 % des gesamten Kontingentplatzes.                                                                                                                       |
| `exceeded` | Das verwendete Kontingent hat das gesamte Kontingent überschritten. Neue Dateien oder Ordner können nicht hinzugefügt werden, wenn sie nicht unter dem Betrag für das Gesamtkontingent liegen oder mehr Speicherplatz erworben wird. |



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "quota resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
