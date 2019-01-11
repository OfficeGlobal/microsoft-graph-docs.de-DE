---
title: Ressourcentyp informationalUrl
description: Grundlegende Profilinformationen der Anwendung.
localization_priority: Normal
ms.openlocfilehash: 78fd03a2673b342d1a0c904f521fe5a0f8cba205
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816982"
---
# <a name="informationalurl-resource-type"></a>Ressourcentyp informationalUrl

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Grundlegende Profilinformationen der Anwendung.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|"Marketing"|Zeichenfolge| Link zu marketing Anwendungsseite. Beispielsweise gibt https://www.contoso.com/app/marketing |
|Datenschutz|Zeichenfolge| Link zu Datenschutzrichtlinie für die Anwendung. Beispielsweise gibt https://www.contoso.com/app/privacy |
|Unterstützung|Zeichenfolge| Link zu der Anwendung Supportseite. Beispielsweise gibt https://www.contoso.com/app/support |
|termsOfService|Zeichenfolge| Link zu der Anwendung Begriffe der Service-Anweisung. Beispielsweise gibt https://www.contoso.com/app/termsofservice |

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
