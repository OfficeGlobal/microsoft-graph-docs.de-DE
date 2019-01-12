---
title: Verwendungsberichte für SharePoint-Website
description: Sie können den Wert eine Ansicht auf oberster Ebene abrufen, die Sie von SharePoint im Hinblick auf die Gesamtzahl der Dateien, die Benutzer in SharePoint-Websites erhalten, wie viele Dateien aktiv verwendet werden und den Speicher für alle diese Websites verbraucht speichern. Anschließend können Sie in der SharePoint-Websiteverwendungsbericht zu verstehen, die Trends und pro Ebene Standortdetails für alle Websites anzeigen.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 964ec64a2cbb15d639a619cf8debd5fb5875245e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950529"
---
# <a name="sharepoint-site-usage-reports"></a>Verwendungsberichte für SharePoint-Website

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
