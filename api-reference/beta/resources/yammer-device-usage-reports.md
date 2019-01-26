---
title: Verwendungsberichte für Yammer-Gerät
description: Die Verwendungsberichte für das Yammer-Gerät geben Aufschluss darüber, welche Geräte Ihre Benutzer für die Nutzung von Yammer verwenden. Sie können sich die Anzahl der Benutzer nach Gerätetyp für einen gewählten Zeitraum ansehen und Details für einzelne Benutzer anzeigen.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 57dcba3a91b15b4980d9e76b7aad6251008f5966
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577431"
---
# <a name="yammer-device-usage-reports"></a>Verwendungsberichte für Yammer-Gerät

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die Verwendungsberichte für das Yammer-Gerät geben Aufschluss darüber, welche Geräte Ihre Benutzer für die Nutzung von Yammer verwenden. Sie können sich die Anzahl der Benutzer nach Gerätetyp für einen gewählten Zeitraum ansehen und Details für einzelne Benutzer anzeigen.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gerätenutzung](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).

## <a name="reports"></a>Berichte

| Function                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getyammerdeviceusageuserdetail.md) | Stream          | [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) | Rufen Sie Details zur Yammer-Gerätenutzung nach Benutzer ab. |
| [Benutzeranzahl für Verteilung abrufen](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Stream          | [yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md) | Erhalten Sie die Anzahl der Benutzer nach Gerätetyp.  |
| [Benutzeranzahl abrufen](../api/reportroot-getyammerdeviceusageusercounts.md) | Stream          | [yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md) | Erhalten Sie die Anzahl der täglichen Benutzer nach Gerätetyp. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
