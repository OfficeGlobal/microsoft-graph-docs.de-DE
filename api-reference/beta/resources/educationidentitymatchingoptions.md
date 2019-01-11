---
title: Ressourcentyp educationIdentityMatchingOptions
description: Stellt eine Zuordnung zwischen einem Source-Eigenschaft und einer Target-Eigenschaft für den Abgleich von Benutzerkonten bereit. Die Source-Eigenschaft sollte in den Quelldaten vorhanden sein. Target-Eigenschaft muss eine gültige Eigenschaft in Azure Active Directory (AD Azure) sein.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 80e9222f8f0c03294a947f403b33cc4f2cd2ef0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876279"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>Ressourcentyp educationIdentityMatchingOptions

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Zuordnung zwischen einem Source-Eigenschaft und einer Target-Eigenschaft für den Abgleich von Benutzerkonten bereit. Die Source-Eigenschaft sollte in den Quelldaten vorhanden sein. Target-Eigenschaft muss eine gültige Eigenschaft in Azure Active Directory (AD Azure) sein.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **appliesTo** | string |  Der Benutzer Rollentyp die Lizenz zugewiesen. Mögliche Werte sind: `student` und `teacher`.      |
| **sourcePropertyName** | string |  Der Name der Source-Eigenschaft, die ein Feldname in den Quelldaten sein sollte. Diese Eigenschaft wird die Groß-/Kleinschreibung beachtet.        |
| **targetPropertyName** | string |  Der Name der Zieleigenschaft, die eine gültige Eigenschaft in Azure AD sein sollte. Diese Eigenschaft wird die Groß-/Kleinschreibung beachtet.     |
| **targetDomain** | string |  Die Domäne, mit der Source-Eigenschaft im Ziel übereinstimmen. Wenn als null angegeben wird, wird die Source-Eigenschaft verwendet werden, der mit der Zieleigenschaft entspricht.        |

## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
