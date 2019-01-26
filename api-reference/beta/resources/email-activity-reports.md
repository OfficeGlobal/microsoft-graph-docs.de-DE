---
title: E-Mail-Aktivitätsberichte
description: Sie können eine Ansicht der e-Mail-Verkehr auf oberster Ebene innerhalb Ihrer Organisation über die Seite Berichte abrufen. Sie können auch in der e-Mail-Aktivität-Widget zu verstehen, die Trends und Details pro Benutzer, der die e-Mail-Aktivität in Ihrer Organisation anzeigen.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: 748199a2e846cc71a3f04c3ea1bda97dcf2c7301
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573900"
---
# <a name="email-activity-reports"></a>E-Mail-Aktivitätsberichte

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie können eine Ansicht der e-Mail-Verkehr auf oberster Ebene innerhalb Ihrer Organisation über die Seite Berichte abrufen. Sie können auch in der e-Mail-Aktivität-Widget zu verstehen, die Trends und Details pro Benutzer, der die e-Mail-Aktivität in Ihrer Organisation anzeigen.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – E-Mail-Aktivität](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).

## <a name="reports"></a>Berichte

| Function                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getemailactivityuserdetail.md) | Stream          | [emailActivityUserDetail](../resources/emailactivityuserdetail.md) | Erhalten Sie detaillierte Informationen über die von Benutzern ausgeführten E-Mail-Aktivitäten. |
| [Aktivitätsanzahl abrufen](../api/reportroot-getemailactivitycounts.md) | Stream          | [emailActivitySummary](../resources/emailactivitysummary.md) | Ermöglicht es Ihnen, einen Überblick über die E-Mail-Aktivitäten (z. B. wie viele E-Mails versendet, gelesen und empfangen wurden) in Ihrer Organisation zu gewinnen. |
| [Benutzeranzahl abrufen](../api/reportroot-getemailactivityusercounts.md) | Stream          | [emailActivitySummary](../resources/emailactivitysummary.md) | Ermöglicht es Ihnen, sich anhand der Anzahl eindeutiger Benutzer, die E-Mail-Aktivitäten wie Senden, Lesen und Empfangen ausführen, über Trends zu informieren. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
