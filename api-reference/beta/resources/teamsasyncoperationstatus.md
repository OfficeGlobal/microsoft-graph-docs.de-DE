---
title: TeamsAsyncOperationStatus Enum-Typ
description: Wird den aktuellen Status der ein TeamsAsyncOperation beschrieben.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e9138adcc646677955a12091a3fb15badfd39f13
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511709"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>TeamsAsyncOperationStatus Enum-Typ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Wird den aktuellen Status der ein [TeamsAsyncOperation](teamsasyncoperation.md)beschrieben.

## <a name="members"></a>Elemente

| Member | Wert| Beschreibung |
|:---------------|:--------|:----------|
|Ungültig|(0)|Ungültiger Wert|
|NotStarted|-1|Der Vorgang wurde nicht gestartet.|
|InProgress|-2|Der Vorgang wird ausgeführt.|
|succeeded|-3|Der Vorgang erfolgreich war.|
|failed|4*|Dieser Vorgang ist fehlgeschlagen.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
