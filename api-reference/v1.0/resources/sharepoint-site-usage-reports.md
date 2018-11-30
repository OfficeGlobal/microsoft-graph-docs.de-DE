---
title: Verwendungsberichte für SharePoint-Website
description: Sie können die Verwendungsberichte für die SharePoint-Website nutzen, um eine allgemeine Übersicht über den Nutzungswert von SharePoint hinsichtlich der Gesamtzahl der Dateien, die Benutzer in SharePoint-Websites speichern, der Anzahl der aktiv genutzten Dateien und des Speicherplatzes, der für all diese Websites verbraucht wird, zu erhalten. Sie können auch einen Drilldown ausführen, um Trends zu erfassen und Details zu den einzelnen Websites zu erhalten.
ms.openlocfilehash: 3f66dde5c351886def3934b4028946a1a837dcc5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016945"
---
# <a name="sharepoint-site-usage-reports"></a>Verwendungsberichte für SharePoint-Website

Sie können die Verwendungsberichte für die SharePoint-Website nutzen, um eine allgemeine Übersicht über den Nutzungswert von SharePoint hinsichtlich der Gesamtzahl der Dateien, die Benutzer in SharePoint-Websites speichern, der Anzahl der aktiv genutzten Dateien und des Speicherplatzes, der für all diese Websites verbraucht wird, zu erhalten. Sie können auch einen Drilldown ausführen, um Trends zu erfassen und Details zu den einzelnen Websites zu erhalten.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Websiteverwendung](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp | Beschreibung                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Websitedetails abrufen](../api/reportroot-getsharepointsiteusagedetail.md) | Stream      | Abrufen von Details zu SharePoint-Websiteverwendung. |
| [Dateianzahl abrufen](../api/reportroot-getsharepointsiteusagefilecounts.md) | Stream      | Rufen Sie die Gesamtzahl der Dateien auf allen Websites und die Anzahl der aktiven Dateien ab. Eine Datei (Benutzer oder System) wird als aktiv betrachtet, wenn sie innerhalb des angegebenen Zeitraums gespeichert, synchronisiert, geändert oder freigegeben wurde. |
| [Websiteanzahl abrufen](../api/reportroot-getsharepointsiteusagesitecounts.md) | Stream      | Rufen Sie die Gesamtzahl der Dateien auf allen Websites und die Anzahl der aktiven Dateien ab. Eine Datei (Benutzer oder System) wird als aktiv betrachtet, wenn sie innerhalb des angegebenen Zeitraums gespeichert, synchronisiert, geändert oder freigegeben wurde. |
| [Speicher abrufen](../api/reportroot-getsharepointsiteusagestorage.md) | Stream      | Erhalten Sie eine Übersicht über den im Berichtszeitraum zugewiesenen und belegten Speicherplatz. |
| [Seiten abrufen](../api/reportroot-getsharepointsiteusagepages.md) | Stream      | Rufen Sie die Anzahl der angezeigten Seiten aller Websites ab. |
