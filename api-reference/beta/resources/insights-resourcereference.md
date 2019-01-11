---
title: Ressourcentyp resourceReference
description: Komplexer Typ mit Eigenschaften des Insights.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 8ab2a79d66db6a45ecf3df748cf8f5740721ef80
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874326"
---
# <a name="resourcereference-resource-type"></a>Ressourcentyp resourceReference

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Komplexer Typ mit Eigenschaften des [Insights](insights.md).

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft      | Typ      | Beschreibung  |
| ------------- |-----------| -------------|
| webUrl        | Zeichenfolge    | Eine URL, die auf das verwiesene Element führende. |
| id            | Zeichenfolge    | Eindeutiger Bezeichner des Elements.           |
| type          | Zeichenfolge    | Ein String-Wert, der verwendet werden kann, um das Element, wie beispielsweise "microsoft.graph.driveItem" klassifizieren |
