---
title: SharePoint-Aktivitätsberichte
description: Sie können die Aktivität jedes Benutzers lizenziert SharePoint verwenden, anhand deren Interaktion mit Dateien abrufen. Sie können sich auch den Umfang der Zusammenarbeit basierend auf der Anzahl der freigegebenen Dateien ansehen.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 98d0393545963a73852197f5bd78241cfb958a22
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577116"
---
# <a name="sharepoint-activity-reports"></a>SharePoint-Aktivitätsberichte

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie können die Aktivität jedes Benutzers lizenziert SharePoint verwenden, anhand deren Interaktion mit Dateien abrufen. Sie können sich auch den Umfang der Zusammenarbeit basierend auf der Anzahl der freigegebenen Dateien ansehen.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Aktivität](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).

## <a name="reports"></a>Berichte

| Function                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getsharepointactivityuserdetail.md) | Stream          | [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) | Rufen Sie Details zu SharePoint-Aktivitäten nach Benutzer ab. |
| [Dateianzahl abrufen](../api/reportroot-getsharepointactivityfilecounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | Erfahren Sie, wie viele eindeutige, lizenzierte Benutzer mit auf SharePoint-Websites gespeicherten Dateien interagiert haben. |
| [Benutzeranzahl abrufen](../api/reportroot-getsharepointactivityusercounts.md) | Stream          | [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) | Rufen Sie die Anzahl der aktiven Benutzer ab. Ein Benutzer wird als aktiv betrachtet, wenn er innerhalb des angegebenen Zeitraums eine Dateiaktivität ausgeführt (speichern, synchronisieren, ändern oder freigeben) oder eine Seite besucht hat. |
| [Seiten abrufen](../api/reportroot-getsharepointactivitypages.md) | Stream          | [sharePointActivityPages](../resources/sharepointactivitypages.md) | Rufen Sie die Anzahl der von Benutzern besuchten eindeutigen Seiten ab. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepoint-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
