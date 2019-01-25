---
title: Microsoft Teams-Gerätenutzungsberichte
description: 'Verwenden Sie die Berichte zur Verwendung der Microsoft-Teams, Gerät, um Einblicke in die Microsoft-Teams Gerät Verwendung in Ihrer Organisation abzurufen. '
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: f9240f6cb310ada94f1a6694efb0da6cd691dc13
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519906"
---
# <a name="microsoft-teams-device-usage-reports"></a>Microsoft Teams-Gerätenutzungsberichte

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Verwenden Sie die Berichte zur Verwendung der Microsoft-Teams, Gerät, um Einblicke in die Microsoft-Teams Gerät Verwendung in Ihrer Organisation abzurufen. 

## <a name="methods"></a>Methoden

| Methode                                   | Rückgabetyp                              | Beschreibung                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getteamsdeviceusageuserdetail.md) | [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) | Abrufen von Details zur Microsoft Teams-Gerätenutzung nach Benutzer. |
| [Benutzeranzahl abrufen](../api/reportroot-getteamsdeviceusageusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | Abrufen der Anzahl der täglichen eindeutigen Benutzer nach Gerätetyp. |
| [Benutzeranzahl für Verteilung abrufen](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | Abrufen der Anzahl der eindeutigen Benutzer nach Gerätetyp im ausgewählten Zeitraum. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
