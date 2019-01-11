---
title: Ressourcentyp educationIdentityDomain
description: 'Stellt die Zuordnung zwischen einer Education Benutzertyp und der Domäne, der das Konto des Benutzers gehört. Die Domänenressource ist Teil der Identity-Konfiguration erstellen. '
localization_priority: Normal
ms.openlocfilehash: 5675499aca010f90deeb517210065ac4802d66b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807749"
---
# <a name="educationidentitydomain-resource-type"></a>Ressourcentyp educationIdentityDomain

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die Zuordnung zwischen einer Education Benutzertyp und der Domäne, der das Konto des Benutzers gehört. Die Domänenressource ist Teil der [Identität Erstellung Konfiguration](educationidentitycreationconfiguration.md). 

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **appliesTo** | string |  Der Benutzer Rollentyp Lizenz zugewiesen. Mögliche Werte sind: `student` und `teacher`.      |
| **name** | string |  Stellt die Domäne für das Benutzerkonto ein.         |

## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "name": "String"
}
```
