---
title: Ressourcentyp educationSynchronizationLicenseAssignment
description: Stellt die Lizenzinformationen Benutzerkonten zugewiesen. Die Ressource wird Lizenz Zuordnungen einrichten, beim Erstellen von neuen Benutzerkonten verwendet werden.
author: mmast-msft
ms.openlocfilehash: 478d939c8f4c6a0bc1971d66afc4ecc7ae640e39
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344394"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a>Ressourcentyp educationSynchronizationLicenseAssignment

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die Lizenzinformationen Benutzerkonten zugewiesen. Die Ressource wird Lizenz Zuordnungen einrichten, beim Erstellen von neuen Benutzerkonten verwendet werden.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **appliesTo** | string | Der Benutzer Rollentyp Lizenz zugewiesen. Mögliche Werte sind: `student` und `teacher`.         |
| **skuIds** | Auflistung von Zeichenfolgen |  Stellt die SKU-Bezeichner, der die Lizenzen zuweisen.        |

## <a name="json-representation"></a>JSON-Darstellung
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
