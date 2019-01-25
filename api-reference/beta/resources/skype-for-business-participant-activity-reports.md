---
title: Aktivitätsbericht für Skype for Business-Teilnehmer
description: Sie können ausführliche Informationen zum Webkonferenz-Aktivität innerhalb Ihrer Organisation erhalten. Diese Details sind sehr hilfreich, wenn Sie andere Geschäftsentscheidungen für Ihre Organisation in Erwägung ziehen, planen und durchführen.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 61c47820febba8f49b98ca19c82d12770da95ce2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516840"
---
# <a name="skype-for-business-participant-activity-reports"></a>Aktivitätsbericht für Skype for Business-Teilnehmer

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie können ausführliche Informationen zum Webkonferenz-Aktivität innerhalb Ihrer Organisation erhalten. Diese Details sind sehr hilfreich, wenn Sie andere Geschäftsentscheidungen für Ihre Organisation in Erwägung ziehen, planen und durchführen.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Konferenzteilnehmeraktivität](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Aktivitätsanzahl abrufen](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | Stream          | [skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md) | Erhalten Sie einen Überblick über die Anzahl und die Art von Konferenzsitzungen, an denen Benutzer aus Ihrer Organisation teilgenommen  haben. Zu den Arten von Konferenzsitzungen gehören Chat, Audio/Video, Anwendungsfreigabe, Web und Einwahl/Auswahl (Drittanbieter). |
| [Benutzeranzahl abrufen](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | Stream          | [skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md) | Erhalten Sie einen Überblick über die Anzahl der eindeutigen Benutzer und die Art von Konferenzsitzungen, an denen Benutzer aus Ihrer Organisation teilgenommen haben. Zu den Arten von Konferenzsitzungen gehören Chat, Audio/Video, Anwendungsfreigabe, Web und Einwahl/Auswahl (Drittanbieter). |
| [Minutenanzahl abrufen](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | Stream          | [skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md) | Erhalten Sie einen Überblick über die Dauer in Minuten und die Art von Konferenzsitzungen, an denen Benutzer aus Ihrer Organisation teilgenommen  haben. Zu den Arten von Konferenzsitzungen gehören Audio/Video. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-participant-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
