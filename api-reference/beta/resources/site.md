---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 1676a314b7c1283918518655b3180cbc70ca193e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952349"
---
# <a name="site-resource-type"></a>Site-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können geändert werden. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **site**-Ressource stellt Metadaten und Beziehungen für eine SharePoint-Website bereit.

## <a name="methods"></a>Methoden

| Method                         | REST-Pfad
|:-------------------------------|:--------------------------------------------
| [Stammwebsite abrufen][]              | GET /sites/root
| [Website abrufen][]                   | GET /sites/{site-id}
| [Website nach Pfad abrufen][]           | GET /sites/{hostname}:/{site-path}
| [Website für eine Gruppe abrufen][]       | GET /groups/{group-id}/sites/root
| [Analysen abrufen][]              | GET /sites/{site-id}/analytics
| [Aktivitäten nach Intervall abrufen][] | GET /sites/{site-id}/getActivitiesByInterval
| [Seiten auflisten][]                 | GET /sites/{site-id}/pages
| [Stammwebsites auflisten][]            | GET /sites?filter=root ne null&select=siteCollection,webUrl
| [Nach Websites suchen][]           | GET /sites?search={query}

[Website abrufen]: ../api/site-get.md
[Stammwebsite abrufen]: ../api/site-get.md
[Website nach Pfad abrufen]: ../api/site-getbypath.md
[Website für eine Gruppe abrufen]: ../api/site-get.md
[Analysen abrufen]: ../api/itemanalytics-get.md
[Aktivitäten nach Intervall abrufen]: ../api/itemactivity-getbyinterval.md
[Seiten auflisten]: ../api/sitepage-list.md
[Stammwebsites auflisten]: ../api/site-list.md
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
| **analytics**     | [itemAnalytics][]-Ressource       | Analysen zu den Anzeigeaktivitäten, die auf dieser Website stattgefunden haben.
| **columns**       | Sammlung ([ColumnDefinition][]) | Die Sammlung der wiederverwendbaren Spaltendefinitionen von Listen unterhalb dieser Website.
| **contentTypes**  | Sammlung ([contentType][])      | Die Sammlung von für diese Website definierten Inhaltstypen.
| **drive**         | [drive][]                        | Das Standardlaufwerk (Dokumentbibliothek) für diese Website.
| **drives**        | Sammlung ([drive][])            | Die Sammlung von Laufwerken (Dokumentbibliotheken) unter dieser Website.
| **items**         | Sammlung ([baseItem][])         | Wird verwendet, um ein beliebiges in dieser Website enthaltenes Element zu adressieren. Diese Sammlung kann nicht aufgezählt werden.
| **Listen**         | Sammlung ([Liste][])             | Die Sammlung der Listen unter dieser Website.
| **pages**         | Sammlung([sitePage][])         | Die Sammlung von Seiten in der SitePages-Liste auf dieser Website.
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
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **site**-Ressource.

Die **site**-Ressource wird von [ **baseItem**](baseitem.md) abgeleitet und erbt Eigenschaften von dieser Ressource.

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
