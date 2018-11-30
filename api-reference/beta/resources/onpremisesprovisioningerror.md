---
title: Ressourcentyp onPremisesProvisioningError
description: Stellt die verzeichnissynchronisierungsfehlern für die Benutzer, Gruppe oder Organisation Kontakt Entitäten bei synchronisieren Verzeichnisse zu Azure Active Directory der lokale.
ms.openlocfilehash: 9fa7850d39c9f7a490135a127938fc7fae30b6f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060788"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>Ressourcentyp onPremisesProvisioningError

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->