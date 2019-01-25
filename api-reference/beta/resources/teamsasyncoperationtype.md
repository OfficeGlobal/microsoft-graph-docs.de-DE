---
title: TeamsAsyncOperationType Enum-Typ
description: Arten von TeamsAsyncOperation. Elemente werden hier wie weitere Async hinzugefügt Vorgänge unterstützt werden.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4de95db194bf41939521b53f06614b46b6afae99
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516567"
---
# <a name="teamsasyncoperationtype-enum-type"></a>TeamsAsyncOperationType Enum-Typ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Arten von [TeamsAsyncOperation](teamsasyncoperation.md). Elemente werden hier wie weitere Async hinzugefügt Vorgänge unterstützt werden.

## <a name="members"></a>Elemente

| Member | Wert| Beschreibung |
|:---------------|:--------|:----------|
|Ungültig|(0)|Ungültiger Wert|
|cloneTeam|-1|Der Vorgang zum Klonen Sie ein Team.|
|archiveTeam|-2|Der Vorgang zum Archivieren von einem Team.|
|unarchiveTeam|-3|Der Vorgang zum Wiederherstellen eines archivierten Teams.|
|createTeam|-3|Vorgang, um ein Team von Grund auf zu erstellen.|

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
