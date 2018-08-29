---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FolderView
ms.openlocfilehash: e73846a18f8576af8fe3cf5949e8ca5c63891837
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265155"
---
# <a name="folderview-resource-type"></a>FolderView-Ressourcentyp

Die **FolderView**-Ressource gibt Empfehlungen zur Benutzerfreundlichkeit eines Ordners oder legt sie fest.

Es ist verfügbar über die Eigenschaft [folder][folder-facet] von Ressourcen des Typs [driveItem][item-resource].

## <a name="json-representation"></a>JSON-Darstellung

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortOrder": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname         | Typ   | Beschreibung
|:----------------------|:-------|:--------------------------------------------
| **sortBy**            | Zeichenfolge | Diese Eigenschaft legt die Methode fest, auf deren Basis der Ordner sortiert werden soll.
| **sortOrder**         | Zeichenfolge | Ist diese Eigenschaft auf „true“ gesetzt, sollen alle Elemente in absteigender Reihenfolge sortiert werden. Andernfalls sollen die Elemente in aufsteigender Reihenfolge sortiert werden.
| **viewType**          | Zeichenfolge | Diese Eigenschaft legt die Ansicht fest, die zur Darstellung des Ordners verwendet werden soll.

Über die Eigenschaft _sortBy_ können Sie die Sortierreihenfolge von Elementen in allen Anwendungen steuern, die das Facet **viewType** berücksichtigen.

### <a name="sortby-options"></a>sortBy-Optionen

Für die Eigenschaft **sortBy** sind die folgenden Werte definiert:

| Wert                    | Beschreibung
| ------------------------ | --------------------------------------------------
| `default`                | Dieser Wert steht für die Standardsortierreihenfolge der Anwendung.
| `name`                   | Elemente sollen auf Basis ihrer Eigenschaft **name** sortiert werden.
| `type`                   | Elemente sollen auf Basis des Elementtyps sortiert werden.
| `size`                   | Elemente sollen auf Basis ihrer Eigenschaft **size** sortiert werden.
| `takenOrCreatedDateTime` | Elemente sollen auf Basis der Eigenschaft **takenDateTime** des Facet **photo** sortiert werden. Ist diese nicht verfügbar, soll die Eigenschaft **createdDateTime** verwendet werden.
| `lastModifiedDateTime`   | Elemente sollen auf Basis ihrer Eigenschaft **lastModifiedDateTime** sortiert werden.
| `sequence`               | Die Elemente folgen einer vom Benutzer angegebenen benutzerdefinierten Sequenz.


### <a name="sortorder-options"></a>sortOrder-Optionen

Für die Eigenschaft **sortOrder** sind die folgenden Werte definiert:

| Wert        | Beschreibung
| ------------ | --------------------------------------------------------------
| `ascending`  | Elemente sollen in aufsteigender Reihenfolge sortiert werden.
| `descending` | Elemente sollen in absteigender Reihenfolge sortiert werden.


### <a name="viewtype-options"></a>viewType-Optionen

Für die Eigenschaft **viewType** sind die folgenden Werte definiert:

| Wert        | Beschreibung
| ------------ | --------------------------------------------------------------
| `default`    | Der Standardansichtstyp der Anwendung
| `icons`      | Eine Ansicht, die Ressourcen des Typs „driveItem“ als Symbole darstellt
| `details`    | Eine Ansicht mit mehreren Spalten, die zusätzliche Details zu den einzelnen Elementen enthalten
| `thumbnails` | Eine Ansicht, die Elemente als größere Miniaturansichten von Ressourcen des Typs „driveItem“ darstellt


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- {
  "type": "#page.annotation",
  "description": "The FolderView facet provides or sets recommendations on the user-experience of a folder.",
  "keywords": "view, folderview, sortby, sortorder, viewtype, coversourceid, folder",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,icons,details,thumbnails) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(default,name,type,size,takenOrCreatedDateTime,lastModifiedDateTime,sequence) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/folderview.md:
      Found potential enums in resource example that weren't defined in a table:(ascending,descending) are in resource, but () are in table"
  ],
  "tocPath": "Facets/FolderView"
} -->
