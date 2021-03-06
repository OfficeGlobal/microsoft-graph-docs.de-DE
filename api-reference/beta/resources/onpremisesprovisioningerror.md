---
title: Ressourcentyp onPremisesProvisioningError
description: Stellt die verzeichnissynchronisierungsfehlern für die Benutzer, Gruppe oder Organisation Kontakt Entitäten bei synchronisieren Verzeichnisse zu Azure Active Directory der lokale.
localization_priority: Normal
ms.openlocfilehash: 7e4d51ea3bde6158256c607027b3e56236a8151c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512731"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>Ressourcentyp onPremisesProvisioningError

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt die verzeichnissynchronisierungsfehlern für die [Benutzer](user.md), [Gruppe](group.md)oder [Organisation Kontakt](orgcontact.md) Entitäten bei synchronisieren Verzeichnisse zu Azure Active Directory der lokale.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|Kategorie|String| Die Kategorie des Fehlers bereitstellen. Hinweis: Zurzeit besteht nur einen möglichen Wert. Wert: *PropertyConflict* - gibt ein Eigenschaftswert ist nicht eindeutig. Andere Objekte enthalten den gleichen Wert für die Eigenschaft. |
|occurredDateTime|DateTimeOffset| Datum und Uhrzeit, an dem der Fehler aufgetreten ist. |
|propertyCausingError|String| Name der Verzeichniseigenschaft den Fehler verursacht. Aktuelle mögliche Werte: *UserPrincipalName* oder *ProxyAddress* |
|Wert|Zeichenfolge| Der Wert der Eigenschaft, die den Fehler verursacht. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesprovisioningerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
