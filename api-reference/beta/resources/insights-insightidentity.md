---
title: insightIdentity
description: " Ressourcentyp"
ms.openlocfilehash: e13d08eb111844896c96b02ab22c52d2f598ce58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062749"
---
# <a name="insightidentity"></a>insightIdentity

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

 Ressourcentyp

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