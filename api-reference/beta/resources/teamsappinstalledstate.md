---
title: Members
description: Wird den aktuelle Installationsstatus von einer TeamsApp beschrieben.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 82e46faccd2a91a82ba4fb7352391f58a42c33a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517274"
---
#<a name="teamsappinstalledstate-enum-type"></a>TeamsAppInstalledState Enum-Typ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Wird den aktuelle Installationsstatus von einer [TeamsApp](teamsapp.md)beschrieben.

## <a name="members"></a>Elemente

| Member | Wert| Beschreibung |
|:---------------|:--------|:----------|
|notInstalled|(0)|App wird an das Team nicht installiert.|
|Installed|-1|App wird normalerweise installiert.|
|installedAndHidden|-2|App wird installiert, jedoch ausgeblendet.|
|installedAndPermanent|-3|App wird dauerhaft installiert und kann nicht entfernt werden.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
