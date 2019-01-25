---
title: ClonableTeamParts Enum-Typ
description: 'Beschreibt, welche Teil eines Teams geklont werden soll. '
localization_priority: Normal
ms.openlocfilehash: 3169d6e367484248e581c12c38887e07cf5c95af
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511464"
---
# <a name="clonableteamparts-enum-type"></a>ClonableTeamParts Enum-Typ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Beschreibt, welche Teil eines [Team](../resources/team.md) geklont werden soll. 

## <a name="members"></a>Elemente

| Member | Wert| Beschreibung |
|:---------------|:--------|:----------|
|Apps|-1|Kopieren Sie die Liste der installierten apps.|
|Registerkarten|-2|die Registerkarten in den Kanälen kopiert.|
|settings|4*|Kopiert alle Einstellungen im Team, zusammen mit den wichtigsten gruppeneinstellungen.|
|Kanäle|8*|kopiert die Struktur DDE-Kanal (jedoch nicht die Nachrichten im Kanal).|
|members|1.6|kopiert die Elemente und Besitzer des Teams.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/clonableteamparts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
