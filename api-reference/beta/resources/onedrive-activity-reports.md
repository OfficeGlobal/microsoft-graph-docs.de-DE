---
title: OneDrive-Aktivitätsberichte
description: Sie können die Aktivität jedes Benutzers OneDrive verwenden, indem Sie deren Interaktion mit Dateien auf OneDrive betrachten lizenziert abrufen. Außerdem können Sie zu verstehen, die Ebene der Zusammenarbeit wie folgt die Anzahl der freigegebenen Dateien fortfahren.
localization_priority: Normal
ms.openlocfilehash: fc87eebeb7c0df1bd6d08a82fa67ccd6d9fa40a8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814490"
---
# <a name="onedrive-activity-reports"></a>OneDrive-Aktivitätsberichte

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Sie können die Aktivität jedes Benutzers OneDrive verwenden, indem Sie deren Interaktion mit Dateien auf OneDrive betrachten lizenziert abrufen. Außerdem können Sie zu verstehen, die Ebene der Zusammenarbeit wie folgt die Anzahl der freigegebenen Dateien fortfahren.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Aktivität](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getonedriveactivityuserdetail.md) | Stream          | [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) | Rufen Sie Details zu OneDrive-Aktivitäten nach Benutzer ab. |
| [Benutzeranzahl abrufen](../api/reportroot-getonedriveactivityusercounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | Rufen Sie die Anzahl der aktiven OneDrive-Benutzer ab. |
| [Dateianzahl abrufen](../api/reportroot-getonedriveactivityfilecounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | Rufen Sie die Anzahl der eindeutigen, lizenzierten Benutzer ab, die Dateiinteraktionen für beliebige OneDrive-Konten ausgeführt haben. |
