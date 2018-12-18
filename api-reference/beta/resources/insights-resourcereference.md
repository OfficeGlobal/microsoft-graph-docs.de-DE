---
title: Ressourcentyp resourceReference
description: Komplexer Typ mit Eigenschaften des Insights.
author: simonhult
ms.openlocfilehash: 2f1a44412eebbb7a74895c12db9a07696d6ee409
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363620"
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
| webUrl        | String    | Eine URL, die auf das verwiesene Element führende. |
| id            | String    | Eindeutiger Bezeichner des Elements.           |
| type          | String    | Ein String-Wert, der verwendet werden kann, um das Element, wie beispielsweise "microsoft.graph.driveItem" klassifizieren |