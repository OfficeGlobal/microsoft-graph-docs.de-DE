# <a name="sharinglink-resource-type"></a>SharingLink-Ressourcentyp

Die **SharingLink**-Ressource gruppiert linkbezogene Datenelemente in einer einzelnen Struktur.

Wenn eine [**Permission**](permission.md)-Ressource ein **sharingLink**-Facet ungleich Null aufweist, stellt die Berechtigung einen Freigabelink dar (im Gegensatz zu Berechtigungen, die einer Person oder Gruppe erteilten werden).

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "type": "view | edit",
  "scope": "anonymous | organization",
  "webUrl": "url"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft    | Typ                    | Beschreibung                                                                                                                                                                                             |
|:------------|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| application | [Identität](identity.md) | Die App, der der Link zugeordnet ist.                                                                                                                                                                    |
| type        | String                  | Der Typ des erstellten Links.                                                                                                                                                                           |
| scope       | String                  | Der Bereich des Links, der durch diese Berechtigung dargestellt wird. Der Wert `anonymous` gibt an, dass der Link von jedem Benutzer verwendet werden kann. `organization` gibt an, dass der Link von Benutzern verwendet werden kann, die bei dem gleichen Mandanten angemeldet sind. |
| webUrl      | String                  | Eine URL, mit der das Element im Browser auf der OneDrive-Website geöffnet wird.                                                                                                                                       |

## <a name="type-enumeration"></a>Type-Enumeration

In dieser Tabelle werden zulässige Werte für die **type**-Eigenschaft aufgeführt:

| Wert   | Funktion    | Beschreibung                                                                     |
|:--------|:--------|:--------------------------------------------------------------------------------|
| `view`  | `read`  | Ein Freigabelink zum Anzeigen für schreibgeschützten Zugriff.                            |
| `edit`  | `write` | Ein Freigabelink zum Bearbeiten für Lese-/Schreibzugriff.                               |

## <a name="scope-enumeration"></a>Scope-Enumeration

| Wert          | Beschreibung                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | Der Freigabelink steht für alle Benutzer zur Verfügung.                                                                            |
| `organization` | Der Freigabelink steht für Benutzer in derselben Organisation (Mandant) zur Verfügung. Nicht für OneDrive Personal verfügbar. |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharingLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
