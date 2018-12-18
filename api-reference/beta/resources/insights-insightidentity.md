---
title: insightIdentity
description: Komplexer Typ, der Eigenschaften von gemeinsamen Elementen enthält.
author: simonhult
ms.openlocfilehash: 648242b827c0390029522955b0fe6347b98100c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331332"
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
| displayName       | String          | Der Anzeigename des Benutzers, der das Element freigegeben. |
| id              | String        | Die Id des Benutzers, der das Element freigegeben.     |
| address             | String      | Die e-Mail-Adresse des Benutzers, der das Element freigegeben werden soll.  |