---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
ms.openlocfilehash: e394d52a5f7ed5e8dce1c61d31d787d62bd36e56
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892337"
---
# <a name="contenttypeinfo-resource-type"></a>ContentTypeInfo-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **ContentTypeInfo**-Ressource gibt den SharePoint-Inhaltstyp eines Elements an.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **contentTypeInfo**-Ressource.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname  | Typ    | Beschreibung
|:---------------|:--------|:--------------------------------------------------
| **id**         | string  | Die ID des Inhaltstyps.
| **name**       | string  | Der Name des Inhaltstyps.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo"
} -->
