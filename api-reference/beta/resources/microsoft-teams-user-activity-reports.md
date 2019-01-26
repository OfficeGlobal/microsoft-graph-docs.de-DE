---
title: Microsoft Teams-Benutzeraktivitätsberichte
description: Verwenden Sie die Microsoft-Teams, Benutzerberichte, um Einblicke in die Microsoft-Teams Benutzeraktivität in Ihrer Organisation abzurufen.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4a071fb38ce9fd76aff4ccdc648201f91a600f24
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574719"
---
# <a name="microsoft-teams-user-activity-reports"></a>Microsoft Teams-Benutzeraktivitätsberichte

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Verwenden Sie die Microsoft-Teams, Benutzerberichte, um Einblicke in die Microsoft-Teams Benutzeraktivität in Ihrer Organisation abzurufen.

## <a name="methods"></a>Methoden

| Methode                                   | Rückgabetyp                              | Beschreibung                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getteamsuseractivityuserdetail.md) | [teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md) | Abrufen von Details zur Microsoft Teams-Benutzeraktivität nach Benutzer. |
| [Aktivitätsanzahl abrufen](../api/reportroot-getteamsuseractivitycounts.md) | [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) | Ruft die Anzahl von Microsoft Teams-Aktivitäten nach Aktivitätstyp ab. Die Aktivitätstypen geben die Anzahl von Chatnachrichten, privaten Chatnachrichten, Anrufen oder Besprechungen der Teams an. |
| [Benutzeranzahl abrufen](../api/reportroot-getteamsuseractivityusercounts.md) | [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) | Ruft die Anzahl der Benutzer nach Aktivitätstyp ab. Die Aktivitätstypen geben die Anzahl von Chatnachrichten, privaten Chatnachrichten, Anrufen oder Besprechungen der Teams an. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-user-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
