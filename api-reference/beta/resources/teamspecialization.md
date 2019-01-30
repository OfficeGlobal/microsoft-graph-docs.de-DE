---
title: TeamSpecialization Enum-Typ
description: Beschreibt den speziellen Anwendungsfall für ein Team.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c89f3ef993e55e28f5558f99c3ef87ad5174bc65
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640322"
---
# <a name="teamspecialization-enum-type"></a>TeamSpecialization Enum-Typ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gibt an, ob das [Team](../resources/team.md) für einen bestimmten Anwendungsfall vorgesehen ist. Jedes [Team](../resources/team.md) Spezialisierung hat Zugriff zur eindeutigen Verhalten und seine Anwendungsfall Ziel Erfahrungen. Standardwert ist "none".

## <a name="members"></a>Elemente

| Element             | Wert | Beschreibung                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| Keine               | 0     | Standard-Typ für ein Team die die standard-Team-Erfahrung haben.          |
| educationStandard  | 1     | Team von einem Benutzer Education erstellt. Alle Teams, Education-Benutzer erstellt, sind vom Typ Edu. |
| educationClass     | 2     | Team optimierte für eine Klasse. Auf diese Weise können Segmentierung des Features across Office 365. |
| educationProfessionalLearningCommunity | 3 | Optimiert für ein PLC Erfahrung im Team. Erfahren Sie mehr über PLC [hier](https://en.wikipedia.org/wiki/Professional_learning_community). |
| educationStaff     | 4     |  Teamtyp für eine optimierte wünschen für Mitarbeiter in einer Organisation, wobei eine Mitarbeiter in leitender Position, wie einem Prinzipal die Admin und Lehrer sind Mitglieder in einem Team, das mit einem speziellen Notizbuch kommt. Weitere Informationen finden Sie unter [Personal OneNote-Notizbuch für Bildungseinrichtungen](https://www.onenote.com/staffnotebookedu). |
| unknownFutureValue | 7     | Sentinel Wert als Platzhalter für zukünftige Erweiterung der Enumeration reserviert. |
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{/api-reference/beta/resources/teamspecialization.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
