---
title: teamsAppInstallation-Ressourcentyp
description: 'Ein teamsApp, das in einem Team installiert ist. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f6ff72ab99d20eba9880630248e4b61fca5c2521
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057015"
---
# <a name="teamsappinstallation-resource-type"></a>teamsAppInstallation-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein [teamsApp](teamsapp.md) , das in einem [Team](team.md)installiert ist. Alle Bots, die Teil der APP sind, werden Teil eines Teams, dem die app hinzugefügt wird.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Apps aufListen](../api/teamsappinstallation-list.md) | [teamsAppInstallation](teamsapp.md) | Listet die in einem Team installierten apps auf.|
|[App hinzufügen](../api/teamsappinstallation-add.md) | [teamsAppInstallation](teamsapp.md) | Hinzufügen (Installieren) einer App zu einem Team.|
|[App entfernen](../api/teamsappinstallation-delete.md) | Keine | Entfernt (deinstalliert) eine APP aus einem Team.|
|[APP aktualisieren](../api/teamsappinstallation-upgrade.md) | Keine | Upgrades auf die neueste Version der app.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ     | Beschreibung |
|:------------------- |:-------- |:----------- |
| id                  | string   | Eine eindeutige ID (nicht die Teams-Kennung). |

## <a name="relationships"></a>Beziehungen

| Beziehung   | Typ    | Beschreibung |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| Die installierte app. |
|teamsAppDefinition|[teamsAppDefinition](teamsapp.md)| Die Details dieser Version der app. |

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a>Siehe auch

- [teamsApp](teamsapp.md)
- [teamsAppDefinition](teamsappdefinition.md)
- [teamsTab](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstallation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

