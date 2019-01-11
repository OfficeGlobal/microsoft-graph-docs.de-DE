---
title: Ressourcentyp teamsAppDefinition
description: Die Details einer Version von einer TeamsApp.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 8a13f6ffd4ca5385b9e264f8b8a5b8bddfe0a1fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851296"
---
# <a name="teamsappdefinition-resource-type"></a>Ressourcentyp teamsAppDefinition

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Details einer Version von einer [TeamsApp](teamsapp.md).

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ     | Beschreibung |
|:------------------- |:-------- |:----------- |
| id                  | string   | Eine eindeutige Id (nicht die Teams Appid). |
| teamsAppId          | string   | Die Id von Teams App-Manifest. |
| displayName         | string   | Der Name der app bereitgestellt von der app-Entwickler. |
| Version             | string   | Die Versionsnummer der Anwendung. |

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0",
}
```

# <a name="see-also"></a>Siehe auch

- [teamsApp](teamsapp.md)
- [teamsAppInstallation](teamsappinstallation.md)
- [teamsTab](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

