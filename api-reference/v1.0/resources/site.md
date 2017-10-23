---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Website
ms.openlocfilehash: db465f93f336a51d862daf6e05b1d6bc422247ea
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="site-resource"></a>Site-Ressource

Die **site**-Ressource stellt Metadaten und Beziehungen für eine SharePoint-Website bereit.

## <a name="tasks"></a>Aufgaben

Alle Beispiele unten beziehen sich auf `https://graph.microsoft.com/v1.0`.

| Aufgabenname                | Beispielanforderung
|:-------------------------|:--------------------------------------------------
| [Stammwebsite abrufen][]        | GET /sites/root
| [Website abrufen][]             | GET /sites/{site-id}
| [Website nach Pfad abrufen][]     | GET /sites/{hostname}:/{site-path}
| [Website für eine Gruppe abrufen][] | GET /groups/{group-id}/sites/root
| [Nach Websites suchen][]     | GET /sites?search={query}

[Website abrufen]: ../api/site_get.md
[Stammwebsite abrufen]: ../api/site_get.md
[Website nach Pfad abrufen]: ../api/site_getbypath.md
[Website für eine Gruppe abrufen]: ../api/site_get.md
[Nach Websites suchen]: ../api/site_search.md

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
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "onenote": [ { "@odata.type": "microsoft.graph.onenote"} ],

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
| **webUrl**               | String (URL)                        | URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.                                          |

## <a name="relationships"></a>Beziehungen

| Beziehungsname | Typ                             | Beschreibung
|:------------------|:---------------------------------|:----------------------
| **columns**       | Sammlung ([ColumnDefinition][]) | Die Sammlung der wiederverwendbaren Spaltendefinitionen von Listen unterhalb dieser Website.
| **contentTypes**  | Sammlung ([contentType][])      | Die Sammlung von für diese Website definierten Inhaltstypen.
| **drive**         | [drive][]                        | Das Standardlaufwerk (Dokumentbibliothek) für diese Website.
| **drives**        | Sammlung ([drive][])            | Die Sammlung von Laufwerken (Dokumentbibliotheken) unter dieser Website.
| **items**         | Sammlung ([baseItem][])         | Wird verwendet, um ein beliebiges in dieser Website enthaltenes Element zu adressieren. Diese Sammlung kann nicht aufgezählt werden.
| **lists**         | Sammlung ([list][])             | Die Sammlung der Listen unter dieser Website.
| **sites**         | Sammlung ([site][])             | Die Sammlung der Unterwebsites unter dieser Website.
| **onenote**       | [onenote][]                      | Ruft den OneNote-Dienst für Notizbuchvorgänge auf.

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contentType.md
[drive]: drive.md
[identitySet]: identityset.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
