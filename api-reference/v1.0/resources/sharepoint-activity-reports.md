---
title: SharePoint-Aktivitätsberichte
description: Verwenden Sie die SharePoint-Aktivitätsberichte, um mehr über die Aktivität der für SharePoint lizenzierten Benutzer zu erfahren, indem Sie sich deren Interaktion mit Dateien ansehen. Sie können sich auch den Umfang der Zusammenarbeit basierend auf der Anzahl der freigegebenen Dateien ansehen.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5754149f573798bfbb10a6ac6c2b9ca60fce597a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575216"
---
# <a name="sharepoint-activity-reports"></a>SharePoint-Aktivitätsberichte

Verwenden Sie die SharePoint-Aktivitätsberichte, um mehr über die Aktivität der für SharePoint lizenzierten Benutzer zu erfahren, indem Sie sich deren Interaktion mit Dateien ansehen. Sie können sich auch den Umfang der Zusammenarbeit basierend auf der Anzahl der freigegebenen Dateien ansehen.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Aktivität](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).

## <a name="reports"></a>Berichte

| Function                                 | Rückgabetyp | Beschreibung                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getsharepointactivityuserdetail.md) | Stream      | Rufen Sie Details zu SharePoint-Aktivitäten nach Benutzer ab. |
| [Dateianzahl abrufen](../api/reportroot-getsharepointactivityfilecounts.md) | Stream      | Erfahren Sie, wie viele eindeutige, lizenzierte Benutzer mit auf SharePoint-Websites gespeicherten Dateien interagiert haben. |
| [Benutzeranzahl abrufen](../api/reportroot-getsharepointactivityusercounts.md) | Stream      | Rufen Sie die Anzahl der aktiven Benutzer ab. Ein Benutzer wird als aktiv betrachtet, wenn er innerhalb des angegebenen Zeitraums eine Dateiaktivität ausgeführt (speichern, synchronisieren, ändern oder freigeben) oder eine Seite besucht hat. |
| [Seiten abrufen](../api/reportroot-getsharepointactivitypages.md) | Stream      | Rufen Sie die Anzahl der von Benutzern besuchten eindeutigen Seiten ab. |
