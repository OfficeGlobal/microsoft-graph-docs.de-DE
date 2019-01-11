---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
ms.openlocfilehash: c7d4b3222ec64432d6a2c9921e53ce409de3f139
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876734"
---
# <a name="contenttype-resource-type"></a>ContentType-Ressourcentyp

Die **ContentType**-Ressource stellt einen _Inhaltstyp_ in SharePoint dar.
Mit Inhaltstypen können Sie eine Reihe von Spalten definieren, die auf jedem [ **ListItem** ] [ listItem] in einer [ **Liste** ] [list] vorhanden sein müssen.

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **contentType**-Ressource.
<!-- {
  "blockType": "resource",
 "baseType": "microsoft.graph.entity",
 "@odata.type": "microsoft.graph.contentType" } -->

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->
