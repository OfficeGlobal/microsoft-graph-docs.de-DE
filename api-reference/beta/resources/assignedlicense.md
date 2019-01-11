---
title: assignedLicense-Ressourcentyp
description: Stellt eine Lizenz dar, die einem Benutzer zugewiesen ist. Die **assignedLicenses**-Eigenschaft der user-Entität ist eine Sammlung von **assignedLicense**.
localization_priority: Normal
ms.openlocfilehash: dfb93075fe62a0cfb479e12554e9078e876c4529
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853783"
---
# <a name="assignedlicense-resource-type"></a>assignedLicense-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Lizenz dar, die einem Benutzer zugewiesen ist. Die **assignedLicenses**-Eigenschaft der [user](user.md)-Entität ist eine Sammlung von **assignedLicense**.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|disabledPlans|GUID-Sammlung|Eine Auflistung der eindeutigen Bezeichner für Pläne, die deaktiviert wurden.|
|skuId|Guid|Die eindeutige ID der SKU.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
