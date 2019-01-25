---
title: Yammer-Gruppenaktivitätsberichte
description: Können Sie Einblicke in die Aktivität des Yammer-Gruppen in Ihrer Organisation erhalten und finden Sie unter wie viele Yammer-Gruppen werden erstellt und verwendet.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 05e5826a85e7d2e37af82cdf6277857746b1b922
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514159"
---
# <a name="yammer-groups-activity-reports"></a>Yammer-Gruppenaktivitätsberichte

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Können Sie Einblicke in die Aktivität des Yammer-Gruppen in Ihrer Organisation erhalten und finden Sie unter wie viele Yammer-Gruppen werden erstellt und verwendet.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gruppenaktivität](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Gruppendetails abrufen](../api/reportroot-getyammergroupsactivitydetail.md) | Stream          | [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) | Rufen Sie Details zur Yammer-Gruppenaktivität nach Gruppe ab. |
| [Gruppenanzahl abrufen](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Stream          | [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) | Erfahren Sie, wie viele Gruppen bisher vorhanden waren und bei wie vielen davon Gruppenunterhaltungsaktivitäten ausgeführt wurden. |
| [Aktivitätsanzahl abrufen](../api/reportroot-getyammergroupsactivitycounts.md) | Stream          | [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) | Rufen Sie die Anzahl der in Gruppen veröffentlichten, gelesenen und gelikten Yammer-Nachrichten ab. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-groups-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
