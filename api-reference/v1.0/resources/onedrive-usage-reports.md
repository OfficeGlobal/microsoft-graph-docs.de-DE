---
title: OneDrive-Verwendungsberichte
description: Mit den OneDrive-Verwendungsberichten können Sie eine allgemeine Übersicht über den durch OneDrive gewonnenen Nutzungswert hinsichtlich der Gesamtzahl der Dateien und des genutzten Speicherplatzes aller OneDrive-Konten in Ihrer Organisation erhalten. Sie können dann ein Drilldown ausführen, um die Trends aktiver OneDrive-Konten zu erfassen und zu erfahren, mit wie vielen Dateien Benutzer interagiert haben und wie viel Speicherplatz verwendet wird. Diese Berichte bieten auch Einzelheiten zu einzelnen OneDrive-Konten.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: fb27d69b3d63fb3f02b4d21e091d44340ec85541
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572402"
---
# <a name="onedrive-usage-reports"></a>OneDrive-Verwendungsberichte

Mit den OneDrive-Verwendungsberichten können Sie eine allgemeine Übersicht über den durch OneDrive gewonnenen Nutzungswert hinsichtlich der Gesamtzahl der Dateien und des genutzten Speicherplatzes aller OneDrive-Konten in Ihrer Organisation erhalten. Sie können dann ein Drilldown ausführen, um die Trends aktiver OneDrive-Konten zu erfassen und zu erfahren, mit wie vielen Dateien Benutzer interagiert haben und wie viel Speicherplatz verwendet wird. Diese Berichte bieten auch Einzelheiten zu einzelnen OneDrive-Konten.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Nutzung](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).

## <a name="reports"></a>Berichte

| Function                                 | Rückgabetyp | Beschreibung                              |
| :--------------------------------------- | :---------- | ---------------------------------------- |
| [Kontodetails abrufen](../api/reportroot-getonedriveusageaccountdetail.md) | Stream      | Rufen Sie Details zur OneDrive-Nutzung nach Konto ab. |
| [Kontoanzahl abrufen](../api/reportroot-getonedriveusageaccountcounts.md) | Stream      | Rufen Sie die Anzahl der aktiven OneDrive for Business-Benutzer ab. Jede Website, über die der Benutzer Dateien angezeigt, geändert, hochgeladen, heruntergeladen, freigegeben oder synchronisiert hat, wird als aktive Website betrachtet. |
| [Dateianzahl abrufen](../api/reportroot-getonedriveusagefilecounts.md) | Stream      | Rufen Sie die Gesamtzahl der Dateien aller Websites und die Anzahl der aktiven Dateien ab. Eine Datei wird als aktiv betrachtet, wenn sie innerhalb des angegebenen Zeitraums gespeichert, synchronisiert, geändert oder freigegeben wurde. |
| [Speicher abrufen](../api/reportroot-getonedriveusagestorage.md) | Stream      | Verschaffen Sie sich einen Überblick über die Menge an Speicherplatz, die Sie in OneDrive for Business verwenden. |
