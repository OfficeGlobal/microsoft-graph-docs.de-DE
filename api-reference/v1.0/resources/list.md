---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Auflisten
ms.openlocfilehash: 3439443090e27c5ef48c2877fe9ea74a9c00cf42
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018387"
---
# <a name="list-resource"></a>List-Ressource

The **list**-Ressource stellt eine Liste auf einer [Website][] dar.
Diese Ressource enthält die Eigenschaften der Liste auf oberster Ebene, einschließlich der Vorlage- und Feld-Definitionen.

## <a name="tasks-on-a-list"></a>Aufgaben in einer Liste

Die folgenden Aufgaben stehen für list-Ressourcen zur Verfügung.
**Hinweis:** Mit dieser Beta können Sie nur durch Listen navigieren, keine Listen erstellen oder aktualisieren.
Sie können jedoch [Listenelemente][listItem] erstellen oder aktualisieren.

Alle Beispiele unten beziehen sich auf  eine Website, z. B.: `https://graph.microsoft.com/v1.0/sites/{site-id}`.

| Häufige Aufgaben               | HTTP-Methode
|:--------------------------|:------------------------------
| [Liste abrufen][]              | GET /lists/{list-id}
| [Listenelemente auflisten][]  | GET /lists/{list-id}/items
| [Listenelement aktualisieren][]      | PATCH /lists/{list-id}/items/{item-id}
| [Listenelement löschen][]      | DELETE /lists/{list-id}/items/{item-id}
| [Listenelement erstellen][]      | POST /lists/{list-id}

[Liste abrufen]: ../api/list-get.md
[Listenelemente auflisten]: ../api/listitem-list.md
[Listenelement aktualisieren]: ../api/listitem-update.md
[Listenelement löschen]: ../api/listitem-delete.md
[Listenelement erstellen]: ../api/listitem-create.md

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **list**-Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "items",
    "drive"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.list"
}-->

```json
{
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "displayName": "title of list",
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "items": [ { "@odata.type": "microsoft.graph.listItem" } ],
  "list": {
    "@odata.type": "microsoft.graph.listInfo",
    "hidden": false,
    "template": "documentLibrary | genericList | survey | links | announcements | contacts | accessRequest ..."
  },
  "system": false,

  /* inherited from baseItem */
  "id": "string",
  "name": "name of list",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of list",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a>Eigenschaften

Die **list**-Ressource besitzt folgende Eigenschaften.

| Eigenschaftsname    | Typ                             | Beschreibung
|:-----------------|:---------------------------------|:---------------------------
| **displayName**  | string                           | Der anzeigbare Titel der Liste.
| **list**         | [listInfo][]                     | Weitere Details über die Liste.
| **system**       | [systemFacet][]                  | Falls vorhanden, gibt an, dass es sich um eine vom System verwaltete Liste handelt. Schreibgeschützt.

Die folgenden Eigenschaften werden von  **[baseItem][]** geerbt.

| Eigenschaftsname            | Typ              | Beschreibung
|:-------------------------|:------------------|:------------------------------
| **id**                   | string            | Der eindeutige Bezeichner des Elements. Schreibgeschützt.
| **name**                 | string            | Der Name des Elements.
| **createdBy**            | [identitySet][]   | Die Identität des Erstellers dieses Elements. Schreibgeschützt.
| **createdDateTime**      | DateTimeOffset    | Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.
| **description**          | string            | Der beschreibende Text für das Element.
| **eTag**                 | string            | ETag für das Element. Schreibgeschützt.                                                          |
| **lastModifiedBy**       | [identitySet][]   | Die Identität derPerson, die dieses Element zuletzt geändert hat. Schreibgeschützt.
| **lastModifiedDateTime** | DateTimeOffset    | Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.
| **parentReference**      | [itemReference][] | Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.
| **sharepointIds**        | [sharepointIds][] | Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.
| **webUrl**               | String (URL)      | URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.

## <a name="relationships"></a>Beziehungen

Die **list**-Ressource weist folgende Beziehungen zu anderen Ressourcen auf.

| Beziehungsname | Typ                             | Beschreibung
|:------------------|:---------------------------------|:----------------------
| **drive**         | [drive][]                        | Nur in Dokumentbibliotheken vorhanden. Ermöglicht den Zugriff auf die Liste als [drive][]-Ressource mit [driveItems][driveItem].
| **items**         | Sammlung ([listItem][])         | Alle in der Liste enthaltenen Elemente.
| **columns**       | Sammlung ([ColumnDefinition][]) | Die Sammlung von Felddefinitionen für diese Liste.
| **contentTypes**  | Sammlung ([contentType][])      | Die Sammlung von in dieser Liste enthaltenen content-Typen.

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[sharepointIds]: sharepointids.md
[Website]: site.md
[systemFacet]: systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists": "#"
  }
} -->
