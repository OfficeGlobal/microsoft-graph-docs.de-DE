---
title: Ressourcentyp onPremisesExtensionAttributes
description: Die **OnPremisesExtensionAttributes** -Eigenschaft der Benutzerentität enthält fünfzehn Eigenschaften der benutzerdefinierten Erweiterung-Attribut. Diese Gruppe von Eigenschaften ist für einen Benutzer **OnPremisesSyncEnabled** im lokalen Active Directory gesteuert und Azure AD synchronisiert und ist schreibgeschützt. Für einen nur-Cloud-Benutzer (wobei **OnPremisesSyncEnabled** ist false), können diese Eigenschaften festgelegt werden, während der Erstellung oder zu aktualisieren.
localization_priority: Normal
ms.openlocfilehash: c0cb765efe9e94c8254e45eaa9d55bc16382f6d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824745"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Ressourcentyp onPremisesExtensionAttributes

Die **OnPremisesExtensionAttributes** -Eigenschaft der [Benutzer](user.md) Entität enthält fünfzehn Eigenschaften der benutzerdefinierten Erweiterung-Attribut. Diese Gruppe von Eigenschaften ist für einen Benutzer **OnPremisesSyncEnabled** im lokalen Active Directory gesteuert und Azure AD synchronisiert und ist schreibgeschützt. Für einen nur-Cloud-Benutzer (wobei **OnPremisesSyncEnabled** ist false), können diese Eigenschaften festgelegt werden, während der Erstellung oder zu aktualisieren.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|extensionAttribute1|Zeichenfolge| Erste anpassbare Extension-Attribut. |
|extensionAttribute2|Zeichenfolge| Zweite anpassbare Extension-Attribut. |
|extensionAttribute3|Zeichenfolge| Dritte anpassbare Extension-Attribut. |
|extensionAttribute4|Zeichenfolge| Vierte anpassbare Extension-Attribut. |
|extensionAttribute5|Zeichenfolge| Fünfte anpassbare Extension-Attribut. |
|extensionAttribute6|Zeichenfolge| Sechste anpassbare Extension-Attribut. |
|extensionAttribute7|Zeichenfolge| Siebte anpassbare Extension-Attribut. |
|extensionAttribute8|Zeichenfolge| Achte anpassbare Extension-Attribut. |
|extensionAttribute9|Zeichenfolge| Neunte anpassbare Extension-Attribut. |
|extensionAttribute10|Zeichenfolge| Zehnte anpassbare Extension-Attribut. |
|extensionAttribute11|Zeichenfolge| Elfte anpassbare Extension-Attribut. |
|extensionAttribute12|Zeichenfolge| Zwölfte anpassbarer Extension-Attribut. |
|extensionAttribute13|Zeichenfolge| Dreizehnte anpassbare Extension-Attribut. |
|extensionAttribute14|Zeichenfolge| Vierzehnte anpassbare Extension-Attribut. |
|extensionAttribute15|Zeichenfolge| Fünfzehnte anpassbare Extension-Attribut. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
