---
title: Yammer-Gruppenaktivitätsberichte
description: Können Sie Einblicke in die Aktivität des Yammer-Gruppen in Ihrer Organisation erhalten und finden Sie unter wie viele Yammer-Gruppen werden erstellt und verwendet.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: e2726e55e089aa494eaf35d0948f0fa3948be781
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950816"
---
# <a name="yammer-groups-activity-reports"></a>Yammer-Gruppenaktivitätsberichte

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt. Diese APIs werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt.

Können Sie Einblicke in die Aktivität des Yammer-Gruppen in Ihrer Organisation erhalten und finden Sie unter wie viele Yammer-Gruppen werden erstellt und verwendet.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gruppenaktivität](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Gruppendetails abrufen](../api/reportroot-getyammergroupsactivitydetail.md) | Stream          | [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) | Rufen Sie Details zur Yammer-Gruppenaktivität nach Gruppe ab. |
| [Gruppenanzahl abrufen](../api/reportroot-getyammergroupsactivitygroupcounts.md) | Stream          | [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) | Erfahren Sie, wie viele Gruppen bisher vorhanden waren und bei wie vielen davon Gruppenunterhaltungsaktivitäten ausgeführt wurden. |
| [Aktivitätsanzahl abrufen](../api/reportroot-getyammergroupsactivitycounts.md) | Stream          | [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) | Rufen Sie die Anzahl der in Gruppen veröffentlichten, gelesenen und gelikten Yammer-Nachrichten ab. |
