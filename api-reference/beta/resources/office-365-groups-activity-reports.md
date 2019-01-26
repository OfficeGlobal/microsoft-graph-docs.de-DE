---
title: Office 365-Gruppenaktivitätsberichte
description: Können Sie Einblicke in die Aktivität des Office 365-Gruppen in Ihrer Organisation erhalten und finden Sie unter wie viele Office 365-Gruppen werden erstellt und verwendet.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e698a1096d244b864bbb15cf06c16e8cf79ff1f2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572199"
---
# <a name="office-365-groups-activity-reports"></a>Office 365-Gruppenaktivitätsberichte

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Können Sie Einblicke in die Aktivität des Office 365-Gruppen in Ihrer Organisation erhalten und finden Sie unter wie viele Office 365-Gruppen werden erstellt und verwendet.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Office 365-Gruppen](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

## <a name="reports"></a>Berichte

| Function                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Gruppendetails abrufen](../api/reportroot-getoffice365groupsactivitydetail.md) | Stream          | [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) | Rufen Sie Details zur Office 365-Gruppenaktivität nach Gruppe ab. |
| [Aktivitätsanzahl abrufen](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) | Rufen Sie die Anzahl der Gruppenaktivitäten für Gruppenarbeitslasten ab. |
| [Gruppenanzahl abrufen](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Stream          | [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) | Erhalten Sie die Gesamtzahl der Gruppen pro Tag und erfahren Sie, wie viele dieser Gruppen durch E-Mail-Unterhaltungen, Yammer-Beiträge und SharePoint-Dateiaktivitäten aktiv waren. |
| [Speicher abrufen](../api/reportroot-getoffice365groupsactivitystorage.md) | Stream          | [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) | Rufen Sie den insgesamt für alle Gruppenpostfächer und Gruppenwebsites genutzten Speicherplatz ab. |
| [Dateianzahl abrufen](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) | Rufen Sie die Gesamtzahl der Dateien ab und erfahren Sie, wie viele der Dateien in allen Office 365-Gruppen zugeordneten Gruppenwebsites aktiv waren. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-groups-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
