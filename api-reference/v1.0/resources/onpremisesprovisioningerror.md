---
title: Ressourcentyp onPremisesProvisioningError
description: Stellt verzeichnissynchronisierungsfehlern für die Benutzer- und Entitäten dar, bei der lokalen Verzeichnisse zu Azure Active Directory-Synchronisierung.
localization_priority: Normal
ms.openlocfilehash: c8989a78dfb60a6c7c25a66a9f1e619dcbdca15d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830667"
---
# <a name="onpremisesprovisioningerror-resource-type"></a>Ressourcentyp onPremisesProvisioningError

Stellt die verzeichnissynchronisierungsfehlern für die [ [Benutzer-](user.md) und](group.md) Entitäten bei synchronisieren Verzeichnisse zu Azure Active Directory der lokale.

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
