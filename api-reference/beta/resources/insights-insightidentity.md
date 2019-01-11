---
title: insightIdentity
description: Komplexer Typ, der Eigenschaften von gemeinsamen Elementen enthält.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 395c865a38ebe6ea84dc64857f441cd529e4f2d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886576"
---
# <a name="insightidentity"></a>insightIdentity

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Komplexer Typ, der Eigenschaften von [gemeinsamen](insights-shared.md) Elementen enthält. 

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft              | Typ          | Beschreibung  |
| -------------         |-----------    | -------------|
| displayName       | Zeichenfolge          | Der Anzeigename des Benutzers, der das Element freigegeben. |
| id              | Zeichenfolge        | Die Id des Benutzers, der das Element freigegeben.     |
| address             | Zeichenfolge      | Die e-Mail-Adresse des Benutzers, der das Element freigegeben werden soll.  |
