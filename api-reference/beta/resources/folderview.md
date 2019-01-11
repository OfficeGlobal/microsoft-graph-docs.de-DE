---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: 717dd93d82f109926cabf0168e4e176d7c68cd35
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861537"
---
# <a name="folderview-resource-type"></a>FolderView-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **FolderView**-Ressource gibt Empfehlungen zur Benutzerfreundlichkeit eines Ordners oder legt sie fest.

Es ist verfügbar über die Eigenschaft [folder][folder-facet] von Ressourcen des Typs [driveItem][item-resource].

## <a name="json-representation"></a>JSON-Darstellung

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.folderView" } -->

```json
{
  "sortBy": "default | name | type | size | takenOrCreatedDateTime | lastModifiedDateTime | sequence",
  "sortDescending": "ascending | descending",
  "viewType": "default | icons | details | thumbnails"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname         | Typ   | Beschreibung
|:----------------------|:-------|:--------------------------------------------
| **sortBy**            | string | Diese Eigenschaft legt die Methode fest, auf deren Basis der Ordner sortiert werden soll.
| **sortOrder**         | string | Ist diese Eigenschaft auf „true“ gesetzt, sollen alle Elemente in absteigender Reihenfolge sortiert werden. Andernfalls sollen die Elemente in aufsteigender Reihenfolge sortiert werden.
| **viewType**          | string | Diese Eigenschaft legt die Ansicht fest, die zur Darstellung des Ordners verwendet werden soll.

Über die Eigenschaft _sortBy_ können Sie die Sortierreihenfolge von Elementen in allen Anwendungen steuern, die das Facet **viewType** berücksichtigen.

### <a name="sortby-values"></a>Werte für „sortBy“

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


### <a name="sortorder-values"></a>sortOrder-Werte

Für die Eigenschaft **sortOrder** sind die folgenden Werte definiert:

| Wert        | Beschreibung
| ------------ | --------------------------------------------------------------
| `ascending`  | Elemente sollen in aufsteigender Reihenfolge sortiert werden.
| `descending` | Elemente sollen in absteigender Reihenfolge sortiert werden.


### <a name="viewtype-values"></a>Werte für „viewType“

Für die Eigenschaft **viewType** sind die folgenden Werte definiert:

| Wert        | Beschreibung
| ------------ | --------------------------------------------------------------
| `default`    | Der Standardansichtstyp der Anwendung
| `icons`      | Eine Ansicht, die Ressourcen des Typs „driveItem“ als Symbole darstellt
| `details`    | Eine Ansicht mit mehreren Spalten, die zusätzliche Details zu den einzelnen Elementen enthalten
| `thumbnails` | Eine Ansicht, die Elemente als größere Miniaturansichten von Ressourcen des Typs „driveItem“ darstellt


[item-resource]: driveitem.md
[folder-facet]: folder.md

<!-- uuid: f9e446fd-190b-4692-a605-bb60e78f1f19
2017-05-03 02:34:40 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
