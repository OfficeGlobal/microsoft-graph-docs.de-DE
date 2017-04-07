# <a name="drive-resource-type"></a>Ressourcentyp drive

Die drive-Ressource ist das Objekt der obersten Ebene innerhalb des OneDrive eines Benutzers oder einer Dokumentbibliothek in SharePoint.

OneDrive-Benutzern steht immer mindestens ein Laufwerk zur Verfügung, das Standardlaufwerk. Benutzern ohne OneDrive-Lizenz steht möglicherweise kein Standardlaufwerk zur Verfügung.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "items", "root", "special" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.drive"
}-->
```json
{
  "id": "string (identifier)",
  "driveType": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "root": {"@odata.type": "microsoft.graph.driveItem" },
  "items": [ {"@odata.type": "microsoft.graph.driveItem" }],
  "special": [ {"@odata.type": "microsoft.graph.driveItem" }]
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft  | Typ                          | Beschreibung                                                                                          |
|:----------|:------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| id        | String                        | Der eindeutige Bezeichner des Laufwerks. Schreibgeschützt.                                                                                                           |
| driveType | String                        | Beschreibt den Typ des Laufwerks, der durch diese Ressource dargestellt wird. Persönliche OneDrive-Laufwerke geben `personal` zurück. OneDrive for Business gibt `business` zurück. SharePoint-Dokumentbibliotheken geben `documentLibrary` zurück. Schreibgeschützt. |
| owner     | [identitySet](identityset.md) | Optional.  Das Benutzerkonto, das das Laufwerk besitzt.                                                                                                                    |
| quota     | [quota](quota.md)             | Optional.  Informationen zum Speicherkontingent des Laufwerks.                                                                                                       |

## <a name="relationships"></a>Beziehungen

| Beziehung | Typ |Beschreibung |
|:--------|:---------------------------|:-------------------------------------------------------------------------|
| items   | [driveitem](driveitem.md) collection | Alle im Laufwerk enthaltenen Elemente. Schreibgeschützt. Lässt Nullwerte zu.                   |
| root    | [driveitem](driveitem.md)            | Der Stammordner des Laufwerks. Schreibgeschützt.                                 |
| Sonderfall | [driveitem](driveitem.md) collection | Sammlung gemeinsamer Ordner, die  in OneDrive zur Verfügung stehen. Schreibgeschützt. Lässt Nullwerte zu. |


## <a name="methods"></a>Methoden

Die folgenden Methoden stehen für Laufwerksressourcen zur Verfügung.

| Methode                                                    | REST-Pfad                            | 
|:----------------------------------------------------------|:-------------------------------------|
| [Abrufen des Standardlaufwerks des Benutzers](../api/drive_get.md)           | `GET /me/drive`                      |
| [Abrufen des Laufwerks eines anderen Benutzers](../api/drive_get.md)           | `GET /users/{user-id}/drive`         |
| [Abrufen des Stammordners für ein Laufwerk](../api/item_get.md)         | `GET /drives/{drive-id}/root`        |
| [Auflisten von Elementen auf einem Laufwerk](../api/item_list_children.md)     | `GET /me/drive/root/children`        |
| [Auflisten von Änderungen auf einem Laufwerk](../api/item_delta.md)           | `GET /me/drive/root/delta`           |
| [Suchen nach Elementen auf einem Laufwerk](../api/item_search.md)          | `GET /me/drive/search(q='text')`     |




<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "drive resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive"
}-->
