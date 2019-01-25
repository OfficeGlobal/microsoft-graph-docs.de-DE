---
title: Ressourcentyp onPremisesExtensionAttributes
description: Die **OnPremisesExtensionAttributes** -Eigenschaft der Benutzerentität enthält fünfzehn Eigenschaften der benutzerdefinierten Erweiterung-Attribut. Bei einem onPremisesSyncEnabled-Benutzer wird dieser Eigenschaftensatz als Master-Datensatz im lokalen Active Directory verwaltet und mit Azure AD synchronisiert. Er ist außerdem schreibgeschützt. Bei einem reinen Cloud-Benutzer (wenn „onPremisesSyncEnabled“ auf „false“ gesetzt ist) können diese Eigenschaften beim Erstellen oder Aktualisieren festgelegt werden.
localization_priority: Normal
ms.openlocfilehash: f44f71fdcd86d2165289282568a2d7153ccc99b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518240"
---
# <a name="onpremisesextensionattributes-resource-type"></a>Ressourcentyp onPremisesExtensionAttributes

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **OnPremisesExtensionAttributes** -Eigenschaft der [Benutzer](user.md) Entität enthält fünfzehn Eigenschaften der benutzerdefinierten Erweiterung-Attribut. Bei einem onPremisesSyncEnabled-Benutzer wird dieser Eigenschaftensatz als Master-Datensatz im lokalen Active Directory verwaltet und mit Azure AD synchronisiert. Er ist außerdem schreibgeschützt. Bei einem reinen Cloud-Benutzer (wenn „onPremisesSyncEnabled“ auf „false“ gesetzt ist) können diese Eigenschaften beim Erstellen oder Aktualisieren festgelegt werden.


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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesextensionattributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
