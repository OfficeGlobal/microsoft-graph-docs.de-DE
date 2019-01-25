---
title: Verwendungsberichte für SharePoint-Website
description: Sie können den Wert eine Ansicht auf oberster Ebene abrufen, die Sie von SharePoint im Hinblick auf die Gesamtzahl der Dateien, die Benutzer in SharePoint-Websites erhalten, wie viele Dateien aktiv verwendet werden und den Speicher für alle diese Websites verbraucht speichern. Anschließend können Sie in der SharePoint-Websiteverwendungsbericht zu verstehen, die Trends und pro Ebene Standortdetails für alle Websites anzeigen.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: f9186c4caca6afe3f96eca8db2c6fc34131f0b98
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508139"
---
# <a name="sharepoint-site-usage-reports"></a>Verwendungsberichte für SharePoint-Website

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie können den Wert eine Ansicht auf oberster Ebene abrufen, die Sie von SharePoint im Hinblick auf die Gesamtzahl der Dateien, die Benutzer in SharePoint-Websites erhalten, wie viele Dateien aktiv verwendet werden und den Speicher für alle diese Websites verbraucht speichern. Anschließend können Sie in der SharePoint-Websiteverwendungsbericht zu verstehen, die Trends und pro Ebene Standortdetails für alle Websites anzeigen.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Websiteverwendung](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Websitedetails abrufen](../api/reportroot-getsharepointsiteusagedetail.md) | Stream          | [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) | Abrufen von Details zu SharePoint-Websiteverwendung. |
| [Dateianzahl abrufen](../api/reportroot-getsharepointsiteusagefilecounts.md) | Stream          | [sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md) | Rufen Sie die Gesamtzahl der Dateien auf allen Websites und die Anzahl der aktiven Dateien ab. Eine Datei (Benutzer oder System) wird als aktiv betrachtet, wenn sie innerhalb des angegebenen Zeitraums gespeichert, synchronisiert, geändert oder freigegeben wurde. |
| [Websiteanzahl abrufen](../api/reportroot-getsharepointsiteusagesitecounts.md) | Stream          | [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md) | Rufen Sie die Gesamtzahl der Dateien auf allen Websites und die Anzahl der aktiven Dateien ab. Eine Datei (Benutzer oder System) wird als aktiv betrachtet, wenn sie innerhalb des angegebenen Zeitraums gespeichert, synchronisiert, geändert oder freigegeben wurde. |
| [Speicher abrufen](../api/reportroot-getsharepointsiteusagestorage.md) | Stream          | [siteUsageStorage](../resources/siteusagestorage.md) | Erhalten Sie eine Übersicht über den im Berichtszeitraum zugewiesenen und belegten Speicherplatz. |
| [Seiten abrufen](../api/reportroot-getsharepointsiteusagepages.md) | Stream          | [sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md) | Rufen Sie die Anzahl der angezeigten Seiten aller Websites ab. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepoint-site-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
