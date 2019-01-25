---
title: OneDrive-Verwendungsberichte
description: Sie können eine grundlegende Übersicht über den Wert abrufen, die Sie aus OneDrive im Hinblick auf die Gesamtzahl der Dateien und allen OneDrive-Konten in Ihrer Organisation verwendeten Speicher erhalten. Sie können dann ein Drilldown ausführen, um die Trends aktiver OneDrive-Konten zu erfassen und zu erfahren, mit wie vielen Dateien Benutzer interagiert haben und wie viel Speicherplatz verwendet wird. Außerdem haben Sie die pro OneDrive Kontodetails.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: c5a73b33f4422440df8817c3f6a69299eedeae50
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519836"
---
# <a name="onedrive-usage-reports"></a>OneDrive-Verwendungsberichte

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie können eine grundlegende Übersicht über den Wert abrufen, die Sie aus OneDrive im Hinblick auf die Gesamtzahl der Dateien und allen OneDrive-Konten in Ihrer Organisation verwendeten Speicher erhalten. Sie können dann ein Drilldown ausführen, um die Trends aktiver OneDrive-Konten zu erfassen und zu erfahren, mit wie vielen Dateien Benutzer interagiert haben und wie viel Speicherplatz verwendet wird. Außerdem haben Sie die pro OneDrive Kontodetails.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Nutzung](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
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
