---
title: Ressourcentyp onPremisesExtensionAttributes
description: Die **OnPremisesExtensionAttributes** -Eigenschaft der Benutzerentität enthält fünfzehn Eigenschaften der benutzerdefinierten Erweiterung-Attribut. Diese Gruppe von Eigenschaften ist für einen Benutzer **OnPremisesSyncEnabled** im lokalen Active Directory gesteuert und Azure AD synchronisiert und ist schreibgeschützt. Für einen nur-Cloud-Benutzer (wobei **OnPremisesSyncEnabled** ist false), können diese Eigenschaften festgelegt werden, während der Erstellung oder zu aktualisieren.
localization_priority: Normal
ms.openlocfilehash: 44589338e25e01cb483df6bfa3c1e078e352f5ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868159"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Ressourcentyp onPremisesExtensionAttributes

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **OnPremisesExtensionAttributes** -Eigenschaft der [Benutzer](user.md) Entität enthält fünfzehn Eigenschaften der benutzerdefinierten Erweiterung-Attribut. Diese Gruppe von Eigenschaften ist für einen Benutzer **OnPremisesSyncEnabled** im lokalen Active Directory gesteuert und Azure AD synchronisiert und ist schreibgeschützt. Für einen nur-Cloud-Benutzer (wobei **OnPremisesSyncEnabled** ist false), können diese Eigenschaften festgelegt werden, während der Erstellung oder zu aktualisieren.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|extensionAttribute1|String| Erste anpassbare Extension-Attribut. |
|extensionAttribute2|String| Zweite anpassbare Extension-Attribut. |
|extensionAttribute3|String| Dritte anpassbare Extension-Attribut. |
|extensionAttribute4|String| Vierte anpassbare Extension-Attribut. |
|extensionAttribute5|String| Fünfte anpassbare Extension-Attribut. |
|extensionAttribute6|String| Sechste anpassbare Extension-Attribut. |
|extensionAttribute7|String| Siebte anpassbare Extension-Attribut. |
|extensionAttribute8|String| Achte anpassbare Extension-Attribut. |
|extensionAttribute9|String| Neunte anpassbare Extension-Attribut. |
|extensionAttribute10|String| Zehnte anpassbare Extension-Attribut. |
|extensionAttribute11|String| Elfte anpassbare Extension-Attribut. |
|extensionAttribute12|String| Zwölfte anpassbarer Extension-Attribut. |
|extensionAttribute13|String| Dreizehnte anpassbare Extension-Attribut. |
|extensionAttribute14|String| Vierzehnte anpassbare Extension-Attribut. |
|extensionAttribute15|String| Fünfzehnte anpassbare Extension-Attribut. |

## <a name="json-representation"></a>JSON-Darstellung

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
