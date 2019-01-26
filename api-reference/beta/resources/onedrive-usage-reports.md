---
title: OneDrive-Verwendungsberichte
description: Sie können eine grundlegende Übersicht über den Wert abrufen, die Sie aus OneDrive im Hinblick auf die Gesamtzahl der Dateien und allen OneDrive-Konten in Ihrer Organisation verwendeten Speicher erhalten. Sie können dann ein Drilldown ausführen, um die Trends aktiver OneDrive-Konten zu erfassen und zu erfahren, mit wie vielen Dateien Benutzer interagiert haben und wie viel Speicherplatz verwendet wird. Außerdem haben Sie die pro OneDrive Kontodetails.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1f899c3a60e1c0d66dd3b7e075bf0daf13de0b43
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574159"
---
# <a name="onedrive-usage-reports"></a>OneDrive-Verwendungsberichte

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie können eine grundlegende Übersicht über den Wert abrufen, die Sie aus OneDrive im Hinblick auf die Gesamtzahl der Dateien und allen OneDrive-Konten in Ihrer Organisation verwendeten Speicher erhalten. Sie können dann ein Drilldown ausführen, um die Trends aktiver OneDrive-Konten zu erfassen und zu erfahren, mit wie vielen Dateien Benutzer interagiert haben und wie viel Speicherplatz verwendet wird. Außerdem haben Sie die pro OneDrive Kontodetails.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Nutzung](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).

## <a name="reports"></a>Berichte

| Function                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | ---------------------------------------- | ---------------------------------------- |
| [Kontodetails abrufen](../api/reportroot-getonedriveusageaccountdetail.md) | Stream          | [oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md) | Rufen Sie Details zur OneDrive-Nutzung nach Konto ab. |
| [Kontoanzahl abrufen](../api/reportroot-getonedriveusageaccountcounts.md) | Stream          | [oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md) | Rufen Sie die Anzahl der aktiven OneDrive for Business-Benutzer ab. Jede Website, über die der Benutzer Dateien angezeigt, geändert, hochgeladen, heruntergeladen, freigegeben oder synchronisiert hat, wird als aktive Website betrachtet. |
| [Dateianzahl abrufen](../api/reportroot-getonedriveusagefilecounts.md) | Stream          | [oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md) | Rufen Sie die Gesamtzahl der Dateien aller Websites und die Anzahl der aktiven Dateien ab. Eine Datei wird als aktiv betrachtet, wenn sie innerhalb des angegebenen Zeitraums gespeichert, synchronisiert, geändert oder freigegeben wurde. |
| [Speicher abrufen](../api/reportroot-getonedriveusagestorage.md) | Stream          | [siteUsageStorage](../resources/siteusagestorage.md) | Verschaffen Sie sich einen Überblick über die Menge an Speicherplatz, die Sie in OneDrive for Business verwenden. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onedrive-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
