---
title: Berichte über aktive Office 365-Benutzer
description: Sie können den Office 365 aktive Benutzer Bericht verwenden, um zu ermitteln, wie viele Lizenzen von Personen in Ihrer Organisation verwendet werden und Ausführen eines Drilldowns Informationen darüber, welche Benutzer welche Produkte verwenden. In diesem Bericht hilft Administratoren nicht ausgelastete Produkte oder Benutzer, die möglicherweise zusätzliche Schulungen oder Informationen zu identifizieren.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: e85924b7066dde92f0db5fd0b3f1f83dd32fd0c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516210"
---
# <a name="office-365-active-users-reports"></a>Berichte über aktive Office 365-Benutzer

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie können den Office 365 aktive Benutzer Bericht verwenden, um zu ermitteln, wie viele Lizenzen von Personen in Ihrer Organisation verwendet werden und Ausführen eines Drilldowns Informationen darüber, welche Benutzer welche Produkte verwenden. In diesem Bericht hilft Administratoren nicht ausgelastete Produkte oder Benutzer, die möglicherweise zusätzliche Schulungen oder Informationen zu identifizieren.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).

## <a name="reports"></a>Berichte
| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getoffice365activeuserdetail.md) | Stream          | [office365ActiveUserDetail](../resources/office365activeuserdetail.md) | Rufen Sie Details zu aktiven Office 365-Benutzern ab. |
| [Benutzeranzahl abrufen](../api/reportroot-getoffice365activeusercounts.md) | Stream          | [office365ActiveUserCounts](../resources/office365activeusercounts.md) | Rufen Sie die Anzahl der im Berichtszeitraum täglich aktiven Benutzer nach Produkt ab. |
| [Benutzeranzahl für Dienste abrufen](../api/reportroot-getoffice365servicesusercounts.md) | Stream          | [office365ServicesUserCounts](../resources/office365servicesusercounts.md) | Rufen Sie die Anzahl der Benutzer nach Aktivitätstyp und Dienst ab. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-active-users-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
