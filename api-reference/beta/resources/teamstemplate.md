---
title: Ressourcentyp teamsTemplate
description: Beschreibt die TeamsTemplate Entität.
author: nkramer
ms.openlocfilehash: b4e32448f864048fdcb54dc001b21b262df2bba3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327713"
---
# <a name="teamstemplate-resource-type"></a>Ressourcentyp teamsTemplate

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Eine Teamvorlage ist eine Vorlage für ein [Team](../resources/team.md) in Microsoft-Teams erstellen. Eine Vorlage gibt die Struktur, Einstellungen und sogar Inhalte, die bereitgestellt werden soll in ein neues Team mit der Vorlage erstellt. Microsoft bietet eine Reihe von Basis Vorlagen und Kunden können ihre eigenen benutzerdefinierten Vorlagen gespeichert.

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ     | Beschreibung |
|:------------------- |:-------- |:----------- |
| id                  | String   | Eindeutiger Bezeichner der Vorlage. Darf nicht null sein. |

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a>Siehe auch

- [Team](team.md)

