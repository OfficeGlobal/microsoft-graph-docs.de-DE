---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Website
ms.openlocfilehash: d18487d9932227df0ce2de3320fcb71ce94ca735
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063905"
---
# <a name="site-resource-type"></a>Website-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **site**-Ressource stellt Metadaten und Beziehungen für eine SharePoint-Website bereit.

## <a name="methods"></a>Methoden

| Methode                         | REST-Pfad
|:-------------------------------|:--------------------------------------------
| [Stammwebsite abrufen][]              | GET /sites/root
| [Website abrufen][]                   | GET /sites/{site-id}
| [Website nach Pfad abrufen][]           | GET /sites/{hostname}:/{site-path}
| [Website für eine Gruppe abrufen][]       | GET /groups/{group-id}/sites/root
| [Abrufen von analytics][]              | GET/Sites / {Site-Id} / Analytics
| [Abrufen von Aktivitäten nach Intervall][] | GET/Sites / {Site-Id} / GetActivitiesByInterval
| [Seiten auflisten][]                 | GET/Sites / {Site-Id} / pages
| [Stamm Websites aufgelistet werden sollen][]            | GET/Sites? Filter = Root Ne null & select = SiteCollection WebUrl
| [Nach Websites suchen][]           | GET /sites?search={query}

[Website abrufen]: ../api/site-get.md
[Stammwebsite abrufen]: ../api/site-get.md
[Website nach Pfad abrufen]: ../api/site-getbypath.md
[Website für eine Gruppe abrufen]: ../api/site-get.md
[Abrufen von analytics]: ../api/itemanalytics-get.md
[Abrufen von Aktivitäten nach Intervall]: ../api/itemactivity-getbyinterval.md
[Seiten auflisten]: ../api/sitepage-list.md
[Stamm Websites aufgelistet werden sollen]: ../api/site-list.md
[Nach Websites suchen]: ../api/site-search.md


## <a name="properties"></a>Eigenschaften

| Eigenschaftenname            | Typ               | Beschreibung
|:-------------------------|:-------------------|:-----------------------------
| **id**                   | string             | Der eindeutige Bezeichner des Elements. Schreibgeschützt.
| **createdDateTime**      | DateTimeOffset     | Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.
| **description**          | string             | Der beschreibende Text für die Website.
| **eTag**                 | string             | ETag für das Element. Schreibgeschützt.                                                                  |
| **displayName**          | string             | Der vollständigen Titel für die Website. Schreibgeschützt.
| **lastModifiedDateTime** | DateTimeOffset     | Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.
| **name**                 | string             | Der Name/Titel des Elements.
| **root**                 | [root][]           | Falls vorhanden, gibt diese Eigenschaft an, dass es sich um die Stammwebsite in der Websitesammlung handelt. Schreibgeschützt.
| **sharepointIds**        | [sharepointIds][]  | Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.
| **siteCollection**       | [siteCollection][] | Stellt Details über die Websitesammlung der Website bereit. Nur für die Stammwebsite verfügbar. Schreibgeschützt.
| **webUrl**               | String (URL)       | URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.

## <a name="relationships"></a>Beziehungen

| Beziehungsname | Typ                             | Beschreibung
|:------------------|:---------------------------------|:----------------------
| **Analytics**     | [ItemAnalytics][] -Ressource       | Analytics über die Aktivitäten anzeigen, die auf dieser Site durchgeführt wurde.
| **columns**       | Sammlung ([ColumnDefinition][]) | Die Sammlung der wiederverwendbaren Spaltendefinitionen von Listen unterhalb dieser Website.
| **contentTypes**  | Sammlung ([contentType][])      | Die Sammlung von für diese Website definierten Inhaltstypen.
| **drive**         | [drive][]                        | Das Standardlaufwerk (Dokumentbibliothek) für diese Website.
| **drives**        | Sammlung ([drive][])            | Die Sammlung von Laufwerken (Dokumentbibliotheken) unter dieser Website.
| **items**         | Sammlung ([baseItem][])         | Wird verwendet, um ein beliebiges in dieser Website enthaltenes Element zu adressieren. Diese Sammlung kann nicht aufgezählt werden.
| **Listen**         | Sammlung ([Liste][])             | Die Sammlung der Listen unter dieser Website.
| **Seiten**         | Auflistung ([SitePage][])         | Die Auflistung von Seiten in der Liste SitePages auf dieser Site.
| **sites**         | Sammlung ([site][])             | Die Sammlung der Unterwebsites unter dieser Website.

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[sitePage]: sitepage.md
[root]: root.md
[Website]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

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
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
