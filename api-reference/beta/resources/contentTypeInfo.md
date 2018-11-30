---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
ms.openlocfilehash: 922f87c77280627efb956e4558e1ff269daa9311
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062457"
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
