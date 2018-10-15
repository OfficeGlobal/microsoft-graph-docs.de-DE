---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Auflisten
ms.openlocfilehash: 9fa1de406a3c4064ccb410b4b5b2df91b54a1bac
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268459"
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

[Liste abrufen]: ../api/list_get.md
[Listenelemente auflisten]: ../api/listitem_list.md
[Listenelement aktualisieren]: ../api/listItem_update.md
[Listenelement löschen]: ../api/listItem_delete.md
[Listenelement erstellen]: ../api/listItem_create.md

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
| **displayName**  | Zeichenfolge                           | Der anzeigbare Titel der Liste.
| **list**         | [listInfo][]                     | Weitere Details über die Liste.
| **system**       | [systemFacet][]                  | Falls vorhanden, gibt an, dass es sich um eine vom System verwaltete Liste handelt. Schreibgeschützt.

Die folgenden Eigenschaften werden von  **[baseItem][]** geerbt.

| Eigenschaftsname            | Typ              | Beschreibung
|:-------------------------|:------------------|:------------------------------
| **ID**                   | Zeichenfolge            | Der eindeutige Bezeichner des Elements. Schreibgeschützt.
| **name**                 | Zeichenfolge            | Der Name des Elements.
| **createdBy**            | [identitySet][]   | Die Identität des Erstellers dieses Elements. Schreibgeschützt.
| **createdDateTime**      | DateTimeOffset    | Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.
| **description**          | Zeichenfolge            | Der beschreibende Text für das Element.
| **eTag**                 | Zeichenfolge            | ETag für das Element. Schreibgeschützt.                                                          |
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

[baseItem]: baseItem.md
[contentType]: contentType.md
[drive]: drive.md
[driveItem]: driveItem.md
[columnDefinition]: columnDefinition.md
[identitySet]: identitySet.md
[itemReference]: itemreference.md
[listInfo]: listInfo.md
[listItem]: listItem.md
[sharepointIds]: sharepointIds.md
[site]: site.md
[systemFacet]: systemFacet.md

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
