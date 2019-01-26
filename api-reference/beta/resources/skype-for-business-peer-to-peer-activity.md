---
title: Skype for Business-Peer-zu-Peer-Aktivitätsberichte
description: Sie können Details für Peer-zu-Peer-Aktivität innerhalb Ihrer Organisation abrufen. Diese Details sind sehr hilfreich, wenn Sie andere Geschäftsentscheidungen für Ihre Organisation in Erwägung ziehen, planen und durchführen.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 8802430e6f2725b520e7b558f48ed760c26b7588
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572416"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a>Skype for Business-Peer-zu-Peer-Aktivitätsberichte

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie können Details für Peer-zu-Peer-Aktivität innerhalb Ihrer Organisation abrufen. Diese Details sind sehr hilfreich, wenn Sie andere Geschäftsentscheidungen für Ihre Organisation in Erwägung ziehen, planen und durchführen.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Peer-to-Peer-Aktivität](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).

## <a name="reports"></a>Berichte

| Function                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Aktivitätsanzahl abrufen](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | Stream          | [skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md) | Erhalten Sie Informationen über die Anzahl und Art der in Ihrem Unternehmen gehaltenen Sitzungen. Zu den Sitzungsarten gehören Chat, Audio, Video, Anwendungsfreigabe und Dateiübertragung. |
| [Benutzeranzahl abrufen](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | Stream          | [skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md) | Erhalten Sie Informationen über die Anzahl der eindeutigen Benutzer und die Art der in Ihrem Unternehmen gehaltenen Peer-to-Peer-Sitzungen. Zu den Sitzungsarten gehören Chat, Audio, Video, Anwendungsfreigabe und Dateiübertragung in Peer-to-Peer-Sitzungen. |
| [Minutenanzahl abrufen](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | Stream          | [skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) | Erhalten Sie Informationen über die Dauer (in Minuten) und die Art der in Ihrem Unternehmen gehaltenen Peer-to-Peer-Sitzungen. Zu den Sitzungsarten gehören Audio und Video. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-peer-to-peer-activity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
