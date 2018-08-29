---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
ms.openlocfilehash: cb16559aa9da3a885be1977bbd1466265d0a72f0
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268333"
---
# <a name="contenttype-resource-type"></a>ContentType-Ressourcentyp

Die **ContentType**-Ressource stellt einen _Inhaltstyp_ in SharePoint dar.
Mit Inhaltstypen können Sie eine Reihe von Spalten definieren, die auf jedem [ **ListItem** ] [ listItem] in einer [ **Liste** ] [list] vorhanden sein müssen.

[list]: list.md
[listItem]: listItem.md

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
| **ID**            | string               | Der eindeutige Bezeichner des Inhaltstyps.
| **inheritedFrom** | [itemReference][]    | Wenn dieses Inhaltstyps aus einem anderen Bereich (z. B. eine Website) übernommen wurde, wird ein Verweis auf das Element angezeigt, in dem der Inhaltstyp definiert ist.
| **name**          | string               | Der Name des Inhaltstyps.
| **order**         | [contentTypeOrder][] | Gibt die Reihenfolge, in welcher der Inhaltstyp in der Auswahl-Benutzeroberfläche angezeigt wird.
| **parentId**      | string               | Der eindeutige Bezeichner des Inhaltstyps.
| **readOnly**      | boolean              | gibt an, dass der Inhaltstyp erst geändert werden kann, nachdem der Wert auf `false` festgelegt wurde.`true`
| **sealed**        | boolean              | gibt an, dass der Inhaltstyp nicht von Benutzern oder über Push-Down-Vorgänge geändert werden kann.`true` Nur Websitesammlungsadministratoren können Inhaltstypen versiegeln oder entsiegeln.

## <a name="relationships"></a>Beziehungen

| Eigenschaftenname   | Typ                      | Beschreibung
|:----------------|:--------------------------|:-------------------------------
| **columnLinks** | [columnLink][]-Sammlung | Die Sammlung von Spalten, die für diesen Inhaltstyp erforderlich sind.

Weitere Informationen finden Sie unter [Einführung in Inhaltstypen und die Inhaltstypveröffentlichung][contentTypeIntro].

[columnLink]: columnLink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemReference.md
[contentTypeOrder]: contentTypeOrder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->
