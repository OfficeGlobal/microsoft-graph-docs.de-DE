---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: edb8d97094b4d26dbbcc008664bf5dfee3a4ddf9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059475"
---
# <a name="columnlink-resource-type"></a>ColumnLink-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

A **ColumnLink** eines [ContentType][] fügt die Website **ColumnDefinition** zu diesem Inhaltstyp hinzu.

[contentType]: contenttype.md

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **columnLink**-Ressource.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname | Typ   | Beschreibung
|:--------------|:-------|:----------------------------------------------------
| **id**        | string | Die eindeutige ID für die Spalte.
| **name**      | string | Der Name der Spalte in diesem Inhaltstyp.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
