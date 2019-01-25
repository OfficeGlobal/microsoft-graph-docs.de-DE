---
title: Ressourcentyp educationIdentityMatchingOptions
description: Stellt eine Zuordnung zwischen einem Source-Eigenschaft und einer Target-Eigenschaft für den Abgleich von Benutzerkonten bereit. Die Source-Eigenschaft sollte in den Quelldaten vorhanden sein. Target-Eigenschaft muss eine gültige Eigenschaft in Azure Active Directory (AD Azure) sein.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 723a74cff1d5a660272d3456e9f54de8a54e21bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513704"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>Ressourcentyp educationIdentityMatchingOptions

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Zuordnung zwischen einem Source-Eigenschaft und einer Target-Eigenschaft für den Abgleich von Benutzerkonten bereit. Die Source-Eigenschaft sollte in den Quelldaten vorhanden sein. Target-Eigenschaft muss eine gültige Eigenschaft in Azure Active Directory (AD Azure) sein.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| appliesTo | string |  Der Benutzer Rollentyp die Lizenz zugewiesen. Mögliche Werte sind: `student` und `teacher`.      |
| **sourcePropertyName** | string |  Der Name der Source-Eigenschaft, die ein Feldname in den Quelldaten sein sollte. Diese Eigenschaft wird die Groß-/Kleinschreibung beachtet.        |
| **targetPropertyName** | string |  Der Name der Zieleigenschaft, die eine gültige Eigenschaft in Azure AD sein sollte. Diese Eigenschaft wird die Groß-/Kleinschreibung beachtet.     |
| **targetDomain** | string |  Die Domäne, mit der Source-Eigenschaft im Ziel übereinstimmen. Wenn als null angegeben wird, wird die Source-Eigenschaft verwendet werden, der mit der Zieleigenschaft entspricht.        |

## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitymatchingoptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
