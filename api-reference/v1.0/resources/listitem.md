---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 0f5afaeff29da6f3a6330975adece44731e014bc
ms.sourcegitcommit: 4bdff5fdaea824c7c1204ec7dd641abc282d32a1
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2018
---
# <a name="listitem-resource"></a>ListItem-Ressource

Diese Ressource stellt ein Element in einer SharePoint-**[Liste][]** dar.
Spaltenwerte in der Liste sind über das `fieldValueSet`-Wörterbuch verfügbar.

## <a name="tasks-on-a-listitem"></a>Aufgaben zu einem listItem

Die folgenden Aufgaben sind für **listItem**-Ressourcen verfügbar.
Alle Beispiele unten beziehen sich auf eine **[Liste][]**, z. B.: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.

| Häufige Aufgaben                    | HTTP-Methode
|:-------------------------------|:------------------------
| [Get][]                        | GET /items/{item-id}
| [Abrufen von Spaltenwerten][Get]       | GET /items/{item-id}?expand=fields
| [Create][]                     | POST /items
| [Delete][]                     | DELETE /items/{item-id}
| [Update][]                     | PATCH /items/{item-id}
| [Aktualisieren von Spaltenwerten][Update] | PATCH /items/{item-id}/fields

[Get]: ../api/listItem_get.md
[Create]: ../api/listItem_create.md
[Delete]: ../api/listItem_delete.md
[Update]: ../api/listItem_update.md

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **listItem**-Ressource.

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.listItem",
       "keyProperty": "id" } -->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentType" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },

  /* relationships */
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "webUrl": "url"
}
```

## <a name="properties"></a>Eigenschaften

Die **listItem**-Ressource weist folgende Eigenschaften auf.

| Eigenschaftsname | Typ                | Beschreibung
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | Der Inhaltstyp dieses Listenelements
| fields        | [fieldValueSet][]   | Die Werte der für dieses Listenelement festgelegten Spalte.

Die folgenden Eigenschaften werden von  ** [baseItem][]** geerbt.

| Eigenschaftsname        | Typ             | Beschreibung
|:---------------------|:-----------------|:-----------------------------------
| id                   | string           | Der eindeutige Bezeichner des Elements. Schreibgeschützt.
| name                 | string           | Der Name/Titel des Elements.
| createdBy            | [identitySet][]  | Die Identität des Erstellers dieses Elements. Schreibgeschützt.
| createdDateTime      | DateTimeOffset   | Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.
| description          | string           | Der beschreibende Text für das Element.
| lastModifiedBy       | [identitySet][]  | Die Identität der Person, die dieses Element zuletzt geändert hat. Schreibgeschützt.
| lastModifiedDateTime | DateTimeOffset   | Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.
| webUrl               | String (URL)     | URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.

## <a name="relationships"></a>Beziehungen

 Die **listItem**-Ressource weist folgende Beziehungen zu anderen Ressourcen auf.

| Beziehungsname | Typ                        | Beschreibung
|:------------------|:----------------------------|:-------------------------------
| driveItem         | [driveItem][]               | Für Dokumentbibliotheken macht die **DriveItem** Beziehung das ListItem als ** [DriveItem][]** verfügbar

[baseItem]: baseItem.md
[contentTypeInfo]: contentTypeInfo.md
[driveItem]: driveItem.md
[fieldValueSet]: fieldValueSet.md
[identitySet]: identitySet.md
[list]: list.md

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
