---
title: Yammer-Aktivitätsberichte
description: Wie viel Aktivität, über die Organisation und die Anzahl der eindeutigen Benutzer, die buchen generiert wird, like und Lesen von Nachrichten auf Yammer, können Sie die Ebene des Engagements mit Yammer Ihrer Organisation vertraut sein.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 252748b639f256467b2a01336488e1df086c69cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509938"
---
# <a name="yammer-activity-reports"></a>Yammer-Aktivitätsberichte

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Wie viel Aktivität, über die Organisation und die Anzahl der eindeutigen Benutzer, die buchen generiert wird, like und Lesen von Nachrichten auf Yammer, können Sie die Ebene des Engagements mit Yammer Ihrer Organisation vertraut sein.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Aktivität](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getyammeractivityuserdetail.md) | Stream          | [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) | Rufen Sie Details zu Yammer-Aktivitäten nach Benutzer ab. |
| [Aktivitätsanzahl abrufen](../api/reportroot-getyammeractivitycounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Gewinnen Sie einen Eindruck der Yammer-Aktivitäten in Ihrer Organisation, indem Sie erfahren, wie viele Nachrichten gepostet, gelesen und gelikt wurden. |
| [Benutzeranzahl abrufen](../api/reportroot-getyammeractivityusercounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Erfahren Sie, wie viele eindeutige Benutzer Yammer-Nachrichten veröffentlicht, gelesen und gelikt haben. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
