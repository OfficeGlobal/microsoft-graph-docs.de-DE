---
title: Ressourcentyp educationIdentityDomain
description: 'Stellt die Zuordnung zwischen einer Education Benutzertyp und der Domäne, der das Konto des Benutzers gehört. Die Domänenressource ist Teil der Identity-Konfiguration erstellen. '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 280ae1a65e0c14e7960d316cc21154e405f2ee0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982029"
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
