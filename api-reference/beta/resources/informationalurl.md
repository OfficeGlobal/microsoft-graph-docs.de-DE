---
title: Ressourcentyp informationalUrl
description: Grundlegende Profilinformationen der Anwendung.
ms.openlocfilehash: c8a13f4f686fe3b6ffd460ab05342b7da9b4a808
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063198"
---
# <a name="informationalurl-resource-type"></a>Ressourcentyp informationalUrl

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Grundlegende Profilinformationen der Anwendung.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|"Marketing"|String| Link zu marketing Anwendungsseite. Beispielsweise gibt https://www.contoso.com/app/marketing |
|Datenschutz|String| Link zu Datenschutzrichtlinie für die Anwendung. Beispielsweise gibt https://www.contoso.com/app/privacy |
|Unterstützung|String| Link zu der Anwendung Supportseite. Beispielsweise gibt https://www.contoso.com/app/support |
|termsOfService|String| Link zu der Anwendung Begriffe der Service-Anweisung. Beispielsweise gibt https://www.contoso.com/app/termsofservice |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationalUrl"
}-->

```json
{
  "marketing": "String",
  "privacy": "String",
  "support": "String",
  "termsOfService": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationalUrl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->