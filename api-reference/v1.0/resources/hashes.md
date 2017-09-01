# <a name="hashes-resource-type"></a>Hash-Ressourcentyp

Die **Hashes**-Ressourcengruppen machen Hashes in einer einzelnen Struktur für ein Element verfügbar.

**Hinweis:** Nicht alle Dienste geben einen Wert für alle aufgeführten Hash-Eigenschaften an.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string",
  "sha1Hash": "string",
  "quickXorHash": "string"
}
```


## <a name="properties"></a>Eigenschaften

| Eigenschaft         | Typ   | Beschreibung                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| **sha1Hash**     | Zeichenfolge | SHA1-Hash für den Inhalt der Datei (sofern zutreffend). Schreibgeschützt. |
| **crc32Hash**    | String | Der Wert der CRC32 der Datei (sofern zutreffend). Schreibgeschützt.            |
| **quickXorHash** | String | Ein proprietärer Hash der Datei, die verwendet werden kann, um festzustellen, ob sich der Inhalt der Datei (sofern zutreffend) geändert hat. Schreibgeschützt. |

**Hinweis:** In einigen Fällen stehen möglicherweise keine Hash-Werte zur Verfügung. Wenn dies der Fall ist, werden die Hash-Werte für ein Element nach dem Download des Elements aktualisiert.


## <a name="remarks"></a>Hinweise

In OneDrive for Business stehen **sha1Hash** und **crc32Hash** nicht zur Verfügung. In OneDrive Personal steht **QuickXorHash** nicht zur Verfügung.

Weitere Informationen über die Facets eines DriveItem finden Sie unter [DriveItem](driveitem.md).


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hashes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
