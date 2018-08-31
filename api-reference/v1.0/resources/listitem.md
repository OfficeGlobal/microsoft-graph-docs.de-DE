---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 13ddb00d90880570361c7dcbe198c7c90e044957
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264399"
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
| [Erstellen][]                     | POST /items
| [Löschen][]                     | DELETE /items/{item-id}
| [Aktualisieren][]                     | PATCH /items/{item-id}
| [Aktualisieren von Spaltenwerten][Update] | PATCH /items/{item-id}/fields

[Get]: ../api/listItem_get.md
[Erstellen]: ../api/listItem_create.md
[Löschen]: ../api/listItem_delete.md
[Aktualisieren]: ../api/listItem_update.md

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

| Eigenschaftennamen | Typ                | Beschreibung
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | Der Inhaltstyp dieses Listenelements

Die folgenden Eigenschaften werden von **[baseItem][]** geerbt.

| Eigenschaftsname        | Typ              | Beschreibung
|:---------------------|:------------------|:----------------------------------
| id                   | Zeichenfolge            | Der eindeutige Bezeichner des Elements. Schreibgeschützt.
| Name                 | Zeichenfolge            | Der Name/Titel des Elements.
| createdBy            | [identitySet][]   | Die Identität des Erstellers dieses Elements. Schreibgeschützt.
| createdDateTime      | DateTimeOffset    | Das Datum und die Uhrzeit der Erstellung des Elements. Schreibgeschützt.
| Beschreibung          | Zeichenfolge            | Der beschreibende Text für das Element.
| eTag                 | Zeichenfolge            | ETag für das Element. Schreibgeschützt.                                                          |
| lastModifiedBy       | [identitySet][]   | Die Identität derPerson, die dieses Element zuletzt geändert hat. Schreibgeschützt.
| lastModifiedDateTime | DateTimeOffset    | Das Datum und die Uhrzeit der letzten Änderung des Elements. Schreibgeschützt.
| parentReference      | [itemReference][] | Informationen zum übergeordneten Element, wenn das Element ein übergeordnetes Element hat. Lese-/Schreibzugriff.
| sharepointIds        | [sharepointIds][] | Gibt Bezeichner zurück, die für SharePoint REST-Kompatibilität nützlich sind. Schreibgeschützt.
| webUrl               | String (URL)      | URL, über die das Element im Browser angezeigt werden kann. Schreibgeschützt.

## <a name="relationships"></a>Beziehungen

 Die **listItem**-Ressource weist folgende Beziehungen zu anderen Ressourcen auf.

| Beziehungsname | Typ                           | Beschreibung
|:------------------|:-------------------------------|:-------------------------------
| driveItem         | [driveItem][]                  | Für Dokumentbibliotheken macht die **DriveItem**-Beziehung das ListItem als ** [DriveItem][]** verfügbar
| Datenfelder            | [fieldValueSet][]              | Die Werte der für dieses Listenelement festgelegten Spalte.
| Versionen          | [ListItemVersion][] -Sammlung | Die Liste der vorherigen Versionen des Listenelements.

[baseItem]: baseItem.md
[contentTypeInfo]: contentTypeInfo.md
[driveItem]: driveItem.md
[fieldValueSet]: fieldValueSet.md
[identitySet]: identitySet.md
[itemReference]: itemreference.md
[Liste]: list.md
[listItemVersion]: listItemVersion.md
[sharepointIds]: sharepointIds.md

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
