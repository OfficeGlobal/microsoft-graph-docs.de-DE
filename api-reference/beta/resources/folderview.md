---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FolderView
localization_priority: Normal
ms.openlocfilehash: e57e74a0dbcb785d88fb7ccdd3aa3c0e62dc882a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517568"
---
# <a name="folderview-resource-type"></a>FolderView-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
<!--
{
  "type": "#page.annotation",
  "description": "folderView resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/folderview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
