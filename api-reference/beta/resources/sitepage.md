---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a756929212dbca04f16e9e4701e34bbd8d4de28f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939238"
---
# <a name="sitepage-resource"></a>SitePage-Ressource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
| [Delete][]                      | Löschen von /pages/ {Seiten-Id}
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
  "webParts": [{ "@odata.type": "microsoft.graph.sitePageWebParts" }],

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
[Website]: site.md
[webPart]: webpart.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  }
} -->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
