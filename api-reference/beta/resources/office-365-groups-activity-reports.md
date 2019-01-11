---
title: Office 365-Gruppenaktivitätsberichte
description: Können Sie Einblicke in die Aktivität des Office 365-Gruppen in Ihrer Organisation erhalten und finden Sie unter wie viele Office 365-Gruppen werden erstellt und verwendet.
localization_priority: Normal
ms.openlocfilehash: 69d1e4e1b52a5221831c5c335c23fe1e1016c398
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850036"
---
# <a name="office-365-groups-activity-reports"></a>Office 365-Gruppenaktivitätsberichte

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Können Sie Einblicke in die Aktivität des Office 365-Gruppen in Ihrer Organisation erhalten und finden Sie unter wie viele Office 365-Gruppen werden erstellt und verwendet.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Office 365-Gruppen](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Gruppendetails abrufen](../api/reportroot-getoffice365groupsactivitydetail.md) | Stream          | [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) | Rufen Sie Details zur Office 365-Gruppenaktivität nach Gruppe ab. |
| [Aktivitätsanzahl abrufen](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) | Rufen Sie die Anzahl der Gruppenaktivitäten für Gruppenarbeitslasten ab. |
| [Gruppenanzahl abrufen](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Stream          | [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) | Erhalten Sie die Gesamtzahl der Gruppen pro Tag und erfahren Sie, wie viele dieser Gruppen durch E-Mail-Unterhaltungen, Yammer-Beiträge und SharePoint-Dateiaktivitäten aktiv waren. |
| [Speicher abrufen](../api/reportroot-getoffice365groupsactivitystorage.md) | Stream          | [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) | Rufen Sie den insgesamt für alle Gruppenpostfächer und Gruppenwebsites genutzten Speicherplatz ab. |
| [Dateianzahl abrufen](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) | Rufen Sie die Gesamtzahl der Dateien ab und erfahren Sie, wie viele der Dateien in allen Office 365-Gruppen zugeordneten Gruppenwebsites aktiv waren. |
