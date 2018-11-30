---
title: Yammer-Gruppenaktivitätsberichte
description: Können Sie Einblicke in die Aktivität des Yammer-Gruppen in Ihrer Organisation erhalten und finden Sie unter wie viele Yammer-Gruppen werden erstellt und verwendet.
ms.openlocfilehash: faaf270d53108892870a32b7c7296b51f0022fea
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061647"
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
