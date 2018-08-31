---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Website
ms.openlocfilehash: 20d31a9cdc0e540c2b2f2d93fedabdc254e9c03e
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265715"
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

Die **site**-Ressource wird von [ **baseItem** ](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "root",
    "sharepointIds",
    "siteCollection",
    "drive",
    "drives",
    "sites"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.site"
}-->

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
  "onenote": { "@odata.type": "microsoft.graph.onenote"},

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
| **ID**                   | Zeichenfolge                              | Der eindeutige Bezeichner des Elements. Schreibgeschützt.                                                  |
| **createdDateTime**      | DateTimeOffset                      | Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.                                             |
| **Beschreibung**          | Zeichenfolge                              | Der beschreibende Text für die Website.                                                             |
| **displayName**          | Zeichenfolge                              | Der vollständigen Titel für die Website. Schreibgeschützt.                                                        |
| **eTag**                 | Zeichenfolge                              | ETag für das Element. Schreibgeschützt.                                                                  |
| **lastModifiedDateTime** | DateTimeOffset                      | Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.                                       |
| **Name**                 | Zeichenfolge                              | Der Name/Titel des Elements.                                                                  |
| **Stamm**                 | [Stamm](root.md)                     | Falls vorhanden, gibt diese Eigenschaft an, dass es sich um die Stammwebsite in der Websitesammlung handelt. Schreibgeschützt.            |
| **sharepointIds**        | [sharepointIds](sharepointids.md)   | Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.                       |
| **siteCollection**       | [siteCollection](sitecollection.md) | Stellt Details über die Websitesammlung der Website bereit. Nur für die Stammwebsite verfügbar. Schreibgeschützt. |
| **webUrl**               | String (URL)                        | URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.                                          |

## <a name="relationships"></a>Beziehungen

| Beziehungsname | Typ                             | Beschreibung
|:------------------|:---------------------------------|:----------------------
| **Spalten**       | Sammlung ([ColumnDefinition][]) | Die Sammlung der wiederverwendbaren Spaltendefinitionen von Listen unterhalb dieser Website.
| **contentTypes**  | Sammlung ([contentType][])      | Die Sammlung von für diese Website definierten Inhaltstypen.
| **Laufwerk**         | [Laufwerk][]                        | Das Standardlaufwerk (Dokumentbibliothek) für diese Website.
| **Laufwerke**        | Sammlung ([drive][])            | Die Sammlung von Laufwerken (Dokumentbibliotheken) unter dieser Website.
| **Elemente**         | Sammlung ([baseItem][])         | Wird verwendet, um ein beliebiges in dieser Website enthaltenes Element zu adressieren. Diese Sammlung kann nicht aufgezählt werden.
| **Listen**         | Sammlung ([Liste][])             | Die Sammlung der Listen unter dieser Website.
| **Sites**         | Sammlung ([site][])             | Die Sammlung der Unterwebsites unter dieser Website.
| **onenote**       | [onenote][]                      | Ruft den OneNote-Dienst für Notizbuchvorgänge auf.

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contentType.md
[Laufwerk]: drive.md
[identitySet]: identityset.md
[Liste]: list.md
[Site]: site.md
[onenote]: onenote.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
