---
title: localeInfo-Ressourcentyp
description: Die Gebietsschemainformationen, einschließlich der bevorzugten Sprache und Land/Region, des angemeldeten Benutzers.
localization_priority: Normal
ms.openlocfilehash: cfd5b0e318a2f78d382dccd10b23da167d8b5c8a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888200"
---
# <a name="localeinfo-resource-type"></a>localeInfo-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Gebietsschemainformationen, einschließlich der bevorzugten Sprache und Land/Region, des angemeldeten Benutzers.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Gebietsschema|string|Eine Gebietsschemadarstellung für den Benutzer, die die bevorzugte Sprache des Benutzers sowie Land/Region umfasst. Z. B. „de-de“. Die Sprachkomponente besteht entsprechend der Definitionen in [ISO 639-1](https://www.iso.org/iso/home/standards/language_codes.htm) aus 2 Buchstaben, und die Länderkomponente besteht entsprechend der Definitionen in [ISO 3166-1-Alpha-2](https://www.iso.org/iso/country_codes.htm) aus 2 Buchstaben.|
|displayName|string|Ein Name, der das Gebietsschema des Benutzers in natürlicher Sprache darstellt, z. B. „Englisch (USA)“.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.localeInfo"
}-->

```json
{
  "locale": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "localeInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
