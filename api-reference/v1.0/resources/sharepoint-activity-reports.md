---
title: SharePoint-Aktivitätsberichte
description: Verwenden Sie die SharePoint-Aktivitätsberichte, um mehr über die Aktivität der für SharePoint lizenzierten Benutzer zu erfahren, indem Sie sich deren Interaktion mit Dateien ansehen. Sie können sich auch den Umfang der Zusammenarbeit basierend auf der Anzahl der freigegebenen Dateien ansehen.
localization_priority: Normal
ms.openlocfilehash: 00cc158fee8b5ec108af99c57c089c2259106a73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869041"
---
# <a name="sharepoint-activity-reports"></a>SharePoint-Aktivitätsberichte

Verwenden Sie die SharePoint-Aktivitätsberichte, um mehr über die Aktivität der für SharePoint lizenzierten Benutzer zu erfahren, indem Sie sich deren Interaktion mit Dateien ansehen. Sie können sich auch den Umfang der Zusammenarbeit basierend auf der Anzahl der freigegebenen Dateien ansehen.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Aktivität](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp | Beschreibung                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getsharepointactivityuserdetail.md) | Stream      | Rufen Sie Details zu SharePoint-Aktivitäten nach Benutzer ab. |
| [Dateianzahl abrufen](../api/reportroot-getsharepointactivityfilecounts.md) | Stream      | Erfahren Sie, wie viele eindeutige, lizenzierte Benutzer mit auf SharePoint-Websites gespeicherten Dateien interagiert haben. |
| [Benutzeranzahl abrufen](../api/reportroot-getsharepointactivityusercounts.md) | Stream      | Rufen Sie die Anzahl der aktiven Benutzer ab. Ein Benutzer wird als aktiv betrachtet, wenn er innerhalb des angegebenen Zeitraums eine Dateiaktivität ausgeführt (speichern, synchronisieren, ändern oder freigeben) oder eine Seite besucht hat. |
| [Seiten abrufen](../api/reportroot-getsharepointactivitypages.md) | Stream      | Rufen Sie die Anzahl der von Benutzern besuchten eindeutigen Seiten ab. |
