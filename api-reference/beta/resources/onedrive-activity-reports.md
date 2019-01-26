---
title: OneDrive-Aktivitätsberichte
description: Sie können die Aktivität jedes Benutzers OneDrive verwenden, indem Sie deren Interaktion mit Dateien auf OneDrive betrachten lizenziert abrufen. Außerdem können Sie zu verstehen, die Ebene der Zusammenarbeit wie folgt die Anzahl der freigegebenen Dateien fortfahren.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d545f1d92beee89e19eb47cfd8c6ba8c391c5349
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574005"
---
# <a name="onedrive-activity-reports"></a>OneDrive-Aktivitätsberichte

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie können die Aktivität jedes Benutzers OneDrive verwenden, indem Sie deren Interaktion mit Dateien auf OneDrive betrachten lizenziert abrufen. Außerdem können Sie zu verstehen, die Ebene der Zusammenarbeit wie folgt die Anzahl der freigegebenen Dateien fortfahren.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Aktivität](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).

## <a name="reports"></a>Berichte

| Function                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getonedriveactivityuserdetail.md) | Stream          | [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) | Rufen Sie Details zu OneDrive-Aktivitäten nach Benutzer ab. |
| [Benutzeranzahl abrufen](../api/reportroot-getonedriveactivityusercounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | Rufen Sie die Anzahl der aktiven OneDrive-Benutzer ab. |
| [Dateianzahl abrufen](../api/reportroot-getonedriveactivityfilecounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | Rufen Sie die Anzahl der eindeutigen, lizenzierten Benutzer ab, die Dateiinteraktionen für beliebige OneDrive-Konten ausgeführt haben. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onedrive-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
