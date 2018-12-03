---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 18ba74fd677c83da5f8bfe5d13303f7b18ed43f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059849"
---
# <a name="listitem-resource"></a>ListItem-Ressource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Diese Ressource stellt ein Element in einer SharePoint-**[Liste][]** dar.
Spaltenwerte in der Liste sind über das `fieldValueSet`-Wörterbuch verfügbar.

## <a name="tasks-on-a-listitem"></a>Aufgaben zu einem listItem

Die folgenden Aufgaben sind für **listItem**-Ressourcen verfügbar.
Alle Beispiele unten beziehen sich auf eine **[Liste][]**, z. B.: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.

| Häufige Aufgaben                    | HTTP-Methode
|:-------------------------------|:------------------------
| [Get][]                        | GET /items/{item-id}
| [Abrufen von Spaltenwerten][Get]       | GET /items/{item-id}?expand=fields
| [Abrufen von analytics][]              | GET-/items/ {Element-Id} / Analytics
| [Abrufen von Aktivitäten nach Intervall][] | GET-/items/ {Element-Id} / GetActivitiesByInterval
| [Create][]                     | POST /items
| [Delete][]                     | DELETE /items/{item-id}
| [Update][]                     | PATCH /items/{item-id}
| [Aktualisieren von Spaltenwerten][Update] | PATCH /items/{item-id}/fields

[Get]: ../api/listitem-get.md
[Abrufen von analytics]: ../api/itemanalytics-get.md
[Abrufen von Aktivitäten nach Intervall]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **listItem**-Ressource.

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.listItem"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "versions": [{"@odata.type": "microsoft.graph.listItemVersion"}],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "url"
}
```

## <a name="properties"></a>Eigenschaften

Die **listItem**-Ressource weist folgende Eigenschaften auf.

| Eigenschaftsname | Typ                | Beschreibung
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | Der Inhaltstyp dieses Listenelements

Die folgenden Eigenschaften werden von  **[baseItem][]** geerbt.

| Eigenschaftsname        | Typ              | Beschreibung
|:---------------------|:------------------|:----------------------------------
| id                   | string            | Der eindeutige Bezeichner des Elements. Schreibgeschützt.
| name                 | string            | Der Name/Titel des Elements.
| createdBy            | [identitySet][]   | Die Identität des Erstellers dieses Elements. Schreibgeschützt.
| createdDateTime      | DateTimeOffset    | Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.
| description          | string            | Der beschreibende Text für das Element.
| eTag                 | string            | ETag für das Element. Schreibgeschützt.                                                          |
| lastModifiedBy       | [identitySet][]   | Die Identität derPerson, die dieses Element zuletzt geändert hat. Schreibgeschützt.
| lastModifiedDateTime | DateTimeOffset    | Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.
| parentReference      | [itemReference][] | Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.
| sharepointIds        | [sharepointIds][] | Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.
| webUrl               | String (URL)      | URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.

## <a name="relationships"></a>Beziehungen

 Die **listItem**-Ressource weist folgende Beziehungen zu anderen Ressourcen auf.

| Beziehungsname | Typ                           | Beschreibung
|:------------------|:-------------------------------|:-------------------------------
| Aktivitäten        | [ItemActivity][]-Sammlung    | Die Liste der letzten Aktivitäten, die für dieses Element durchgeführt wurden.
| Analytics         | [ItemAnalytics][] -Ressource     | Analytics über die Aktivitäten anzeigen, die für dieses Element ausgeführt wurden.
| driveItem         | [driveItem][]                  | Für Dokumentbibliotheken macht die **DriveItem** Beziehung das ListItem als ** [DriveItem][]** verfügbar
| fields            | [fieldValueSet][]              | Die Werte der für dieses Listenelement festgelegten Spalte.
| Versionen          | [ListItemVersion][] -Auflistung | Die Liste der vorherigen Versionen des Listenelements.

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  }
} -->
