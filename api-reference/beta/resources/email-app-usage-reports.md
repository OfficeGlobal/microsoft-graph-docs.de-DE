---
title: E-Mail-App-Verwendungsbericht
description: Sie können sehen, wie viele e-Mail-apps für die Verbindung zu Exchange Online verwendet werden. Sie können auch nachsehen, welche Versionen von Outlook-Apps verwendet werden, sodass Sie Benutzer informieren können, die auf unterstützte Outlook-Versionen upgraden sollten.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 7f332359af9a6147894bb69e6d12532a83394bb5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573746"
---
# <a name="email-app-usage-reports"></a>E-Mail-App-Verwendungsbericht

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie können sehen, wie viele e-Mail-apps für die Verbindung zu Exchange Online verwendet werden. Sie können auch nachsehen, welche Versionen von Outlook-Apps verwendet werden, sodass Sie Benutzer informieren können, die auf unterstützte Outlook-Versionen upgraden sollten.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Nutzung von E-Mail-Apps](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).

## <a name="reports"></a>Berichte

| Function                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getemailappusageuserdetail.md) | Stream          | [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) | Erhalten Sie detaillierte Informationen darüber, welche Aktivitäten Benutzer mit den verschiedenen E-Mail-Apps ausgeführt haben. |
| [Benutzeranzahl für Apps abrufen](../api/reportroot-getemailappusageappsusercounts.md) | Stream          | [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) | Rufen Sie die Anzahl der eindeutigen Benutzer pro E-Mail-App ab. |
| [Benutzeranzahl abrufen](../api/reportroot-getemailappusageusercounts.md) | Stream          | [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) | Rufen Sie die Anzahl der eindeutigen Benutzer ab, die über eine E-Mail-App mit Exchange Online verbunden sind. |
| [Benutzeranzahl für Versionen abrufen](../api/reportroot-getemailappusageversionsusercounts.md) | Stream          | [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) | Rufen Sie die Anzahl der eindeutigen Benutzer der Desktopversion von Outlook ab. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-app-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
