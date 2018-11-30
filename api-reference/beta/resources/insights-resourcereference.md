---
title: Ressourcentyp resourceReference
description: Komplexer Typ mit Eigenschaften des Insights.
ms.openlocfilehash: d171151a1c3547aa6863a7f70cc3a42ddec13e5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062948"
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
| Typ          | String    | Ein String-Wert, der verwendet werden kann, um das Element, wie beispielsweise "microsoft.graph.driveItem" klassifizieren |