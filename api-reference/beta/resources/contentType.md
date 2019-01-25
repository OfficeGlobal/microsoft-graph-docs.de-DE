---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
ms.openlocfilehash: c90dd8889d07f903a7d3c79d9e4e5db3b9f2a30b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522973"
---
# <a name="contenttype-resource-type"></a>ContentType-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **ContentType**-Ressource stellt einen _Inhaltstyp_ in SharePoint dar.
Mit Inhaltstypen können Sie eine Reihe von Spalten definieren, die auf jedem [ **ListItem** ] [ listItem] in einer [ **Liste** ] [list] vorhanden sein müssen.

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **contentType**-Ressource.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType" } -->

```json
{
  "description": "string",
  "group": "string",
  "hidden": false,
  "id": "string",
  "inheritedFrom": { "@type": "microsoft.graph.itemReference" },
  "name": "string",
  "order": { "@type": "microsoft.graph.contentTypeOrder" },
  "parentId": "string",
  "readOnly": false,
  "sealed": false,

  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }]
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname     | Typ                 | Beschreibung
|:------------------|:---------------------|:----------------------------------
| **description**   | string               | Der beschreibende Text für das Element.
| **group**         | string               | Der Name der Gruppe, der dieser Inhaltstyp angehört. Dadurch können dazugehörige Inhaltstypen einfacher organisiert werden.
| **hidden**        | boolean              | Gibt an, ob der Inhaltstyp im Menü 'Neu' der Liste ausgeblendet ist.
| **id**            | string               | Der eindeutige Bezeichner des Inhaltstyps.
| **inheritedFrom** | [itemReference][]    | Wenn dieses Inhaltstyps aus einem anderen Bereich (z. B. eine Website) übernommen wurde, wird ein Verweis auf das Element angezeigt, in dem der Inhaltstyp definiert ist.
| **name**          | string               | Der Name des Inhaltstyps.
| **order**         | [contentTypeOrder][] | Gibt die Reihenfolge, in welcher der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.
| **parentId**      | string               | Der eindeutige Bezeichner des Inhaltstyps.
| **readOnly**      | boolean              | `true` gibt an, dass der Inhaltstyp erst geändert werden kann, nachdem der Wert auf `false` festgelegt wurde.
| **sealed**        | boolean              | `true` gibt an, dass der Inhaltstyp nicht von Benutzern oder über Push-Down-Vorgänge geändert werden kann. Nur Websitesammlungsadministratoren können Inhaltstypen versiegeln oder entsiegeln.

## <a name="relationships"></a>Beziehungen

| Eigenschaftsname   | Typ                      | Beschreibung
|:----------------|:--------------------------|:-------------------------------
| **columnLinks** | [columnLink][]-Sammlung | Die Sammlung von Spalten, die für diesen Inhaltstyp erforderlich sind.

Weitere Informationen finden Sie unter [Einführung in Inhaltstypen und die Inhaltstypveröffentlichung][contentTypeIntro].

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType",
  "suppressions": [
    "Error: /api-reference/beta/resources/contentType.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
