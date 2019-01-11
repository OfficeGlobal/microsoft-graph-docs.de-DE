---
title: Ressourcentyp teamsTemplate
description: Beschreibt die TeamsTemplate Entität.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 6e847c7ef0b13dd9c4281c17939164128be8b6a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818872"
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

