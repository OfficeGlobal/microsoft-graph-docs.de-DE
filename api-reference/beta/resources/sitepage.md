---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9ecc23abbee165bce9fd4d9a2a5d8aac8aa02f41
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576241"
---
# <a name="sitepage-resource"></a>SitePage-Ressource

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Diese Ressource stellt eine Seite in der SitePages [Liste][]dar.
Sie enthält den Titel, Layout und eine Auflistung von [WebPart][]s.

## <a name="tasks-on-a-page"></a>Aufgaben auf einer Seite

Die folgenden Aufgaben sind für **SitePage** Ressourcen verfügbar.
Alle unten stehenden Beispiele sind relativ zu einer [Website][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.

| Häufige Aufgaben                     | HTTP-Methode
|:--------------------------------|:------------------------------
| [Seiten auflisten][]                  | Abrufen von /pages
| [Seite abrufen][]                    | Abrufen von /pages/ {Seiten-Id}
| [Create][]                      | POST-/pages
| [Löschen][]                      | Löschen von /pages/ {Seiten-Id}
| [Publish][]                     | Posten Sie /pages/ {Seiten-Id} / veröffentlichen

[Seiten auflisten]: ../api/sitepage-list.md
[Seite abrufen]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **SitePage** Ressource.

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayout": "Article",
  "webParts": [{ "@odata.type": "microsoft.graph.webPart" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

  /* inherited from baseItem */
  "id": "string",
  "name": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a>Eigenschaften

Die Ressource **SitePage** hat die folgenden Eigenschaften.

| Eigenschaftenname    | Typ                         | Beschreibung
|:-----------------|:-----------------------------|:---------------------------
| contentType      | [contentTypeInfo][]          | Der Inhaltstyp der Seite.

## <a name="page-content"></a>Seiteninhalt

Die Ressource **SitePage** hat die folgenden Felder Content.

| Eigenschaftenname      | Typ                       | Beschreibung
|:-------------------|:---------------------------|:---------------------------
| title              | string                     | Der Titel der Seite.
| pageLayout         | string                     | Der Name des auf der Seite auf das Seitenlayout.
| webParts           | [webPart][]                | Die Webparts auf der Seite.

## <a name="authoring-metadata"></a>Erstellen von Metadaten

Die Ressource **SitePage** hat die folgende authoring-bezogenen Metadaten. Die PublishingState-Eigenschaft wird die Seite Status wie ausgecheckt oder veröffentlicht authoring widerspiegeln.

| Eigenschaftenname          | Typ                   | Beschreibung
|:-----------------------|:-----------------------|:---------------------------
| publishingState        | [publicationFacet][]   | Den Veröffentlichungsstatus und die MM.mm Version der Seite.

Die folgenden Eigenschaften werden von  **[baseItem][]** geerbt.

| Eigenschaftsname        | Typ              | Beschreibung
|:---------------------|:------------------|:----------------------------------
| id                   | string            | Der eindeutige Bezeichner des Elements. Schreibgeschützt.
| name                 | string            | Der Name/Titel des Elements.
| createdBy            | [identitySet][]   | Die Identität des Erstellers dieses Elements. Schreibgeschützt.
| eTag                 | string            | ETag für das Element. Schreibgeschützt.
| lastModifiedBy       | [identitySet][]   | Die Identität derPerson, die dieses Element zuletzt geändert hat. Schreibgeschützt.
| lastModifiedDateTime | DateTimeOffset    | Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.
| parentReference      | [itemReference][] | Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.
| webUrl               | String (URL)      | URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.

## <a name="relationships"></a>Beziehungen

Die Ressource **SitePage** hat keine Beziehung zu anderen Ressourcen.

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md
[site]: site.md
[webPart]: webpart.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/sitepage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
