---
title: TeamSpecialization Enum-Typ
description: Beschreibt den speziellen Anwendungsfall für ein Team.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9e19c6b2242256f0d1b7a23c89aa07787bfc1913
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522651"
---
# <a name="teamspecialization-enum-type"></a>TeamSpecialization Enum-Typ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gibt an, ob das [Team](../resources/team.md) für einen bestimmten Anwendungsfall vorgesehen ist. Jedes [Team](../resources/team.md) Spezialisierung hat Zugriff zur eindeutigen Verhalten und seine Anwendungsfall Ziel Erfahrungen. Standardwert ist "none".

## <a name="members"></a>Elemente

| Member             | Wert | Beschreibung                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| Keine               | (0)     | Standard-Typ für ein Team die die standard-Team-Erfahrung haben.          |
| unknownFutureValue | -7     | Sentinel Wert als Platzhalter für zukünftige Erweiterung der Enumeration reserviert. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamspecialization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
