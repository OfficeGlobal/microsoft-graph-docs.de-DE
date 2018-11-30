---
title: Ressourcentyp educationIdentityDomain
description: 'Stellt die Zuordnung zwischen einer Education Benutzertyp und der Domäne, der das Konto des Benutzers gehört. Die Domänenressource ist Teil der Identity-Konfiguration erstellen. '
ms.openlocfilehash: 8298e1eb38ae70f982719ee3a7d6588cd181bdd8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063349"
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
