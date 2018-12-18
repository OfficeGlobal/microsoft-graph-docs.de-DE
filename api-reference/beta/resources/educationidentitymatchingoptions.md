---
title: Ressourcentyp educationIdentityMatchingOptions
description: Stellt eine Zuordnung zwischen einem Source-Eigenschaft und einer Target-Eigenschaft für den Abgleich von Benutzerkonten bereit. Die Source-Eigenschaft sollte in den Quelldaten vorhanden sein. Target-Eigenschaft muss eine gültige Eigenschaft in Azure Active Directory (AD Azure) sein.
author: mmast-msft
ms.openlocfilehash: bc2b99654d8e27d52ed92d9b55a32fdff8e730f4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325431"
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
