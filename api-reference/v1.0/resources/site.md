# <a name="site-resource"></a>Site-Ressource

Die **site**-Ressource stellt Metadaten und Beziehungen für eine SharePoint-Website bereit.

## <a name="tasks"></a>Aufgaben

Alle Beispiele unten beziehen sich auf `https://graph.microsoft.com/v1.0`.

| Aufgabenname            | Beispielanforderung                                   |
| :------------------- | :------------------------------------------------ |
| [Stammwebsite abrufen][]    | GET /sites/root                                   |
| [Website abrufen][]         | GET /sites/{site-id}                              |
| [Website nach Pfad abrufen][] | GET /sites/{hostname}:/{site-path}                |
| [Website für eine Gruppe abrufen][] | GET /groups/{group-id}/sites/root             |

[Website abrufen]: ../api/site_get.md
[Stammwebsite abrufen]: ../api/site_get.md
[Website nach Pfad abrufen]: ../api/site_get.md
[Website für eine Gruppe abrufen]: ../api/site_get.md

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **site**-Ressource.

Die **driveItem**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.

<!-- { "blockType": "resource",
       "@odata.type": "microsoft.graph.site",
       "keyProperty": "id",
       "optionalProperties": [ "root", "sharepointIds", "siteCollection", "drive", "drives", "sites" ] } -->

```json
{
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},
  "displayName": "string",

  /* relationships */
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname            | Typ                                | Beschreibung                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| **id**                   | string                              | Der eindeutige Bezeichner des Elements. Schreibgeschützt.                                                  |
| **createdDateTime**      | DateTimeOffset                      | Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.                                             |
| **description**          | string                              | Der beschreibende Text für die Website.                                                             |
| **displayName**          | string                              | Der vollständigen Titel für die Website. Schreibgeschützt.                                                        |
| **lastModifiedDateTime** | DateTimeOffset                      | Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.                                       |
| **name**                 | string                              | Der Name/Titel des Elements.                                                                  |
| **root**                 | [root](root.md)                     | Falls vorhanden, gibt diese Eigenschaft an, dass es sich um die Stammwebsite in der Websitesammlung handelt. Schreibgeschützt.            |
| **sharepointIds**        | [sharepointIds](sharepointids.md)   | Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.                       |
| **siteCollection**       | [siteCollection](sitecollection.md) | Stellt Details über die Websitesammlung der Website bereit. Nur für die Stammwebsite verfügbar. Schreibgeschützt. |
| **webUrl**               | string (URL)                        | URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.                                          |

## <a name="relationships"></a>Beziehungen

| Beziehungsname | Typ                     | Beschreibung
|:------------------|:-------------------------|:----------------------------------
| **drive**         | [drive][]                | Das Standardlaufwerk (Dokumentbibliothek) für diese Website.
| **drives**        | Sammlung ([drive][])    | Die Sammlung von Laufwerken (Dokumentbibliotheken) unter dieser Website.
| **items**         | Sammlung ([baseItem][]) | Wird verwendet, um ein beliebiges in dieser Website enthaltenes Element zu adressieren. Diese Sammlung kann nicht aufgezählt werden.
| **sites**         | Sammlung ([site][])     | Die Sammlung der Unterwebsites unter dieser Website.

[baseItem]: baseitem.md
[drive]: drive.md
[identitySet]: identityset.md
[site]: site.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Site",
  "tocBookmarks": {
    "Site": "#"
  }
} -->
