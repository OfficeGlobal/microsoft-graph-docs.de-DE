---
title: Postfach-Verwendungsberichte
description: Sie erhalten Informationen zu Benutzern mit einem Postfach und ihrer Ebene der Aktivität, die in erster Linie auf gesendeten und empfangenen e-Mails basiert. Sie können auch sehen, wie viel Speicherplatz jedes Postfach beansprucht und wie viele Postfächer sich den  Speicherkontingenten nähern.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: reports
ms.openlocfilehash: ae0b3294750271f32d91dca79f75e7cf44641045
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576325"
---
# <a name="mailbox-usage-reports"></a>Postfach-Verwendungsberichte

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Sie erhalten Informationen zu Benutzern mit einem Postfach und ihrer Ebene der Aktivität, die in erster Linie auf gesendeten und empfangenen e-Mails basiert. Sie können auch sehen, wie viel Speicherplatz jedes Postfach beansprucht und wie viele Postfächer sich den  Speicherkontingenten nähern.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Postfachnutzung](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).

## <a name="reports"></a>Berichte

| Function                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Postfachdetails abrufen](../api/reportroot-getmailboxusagedetail.md) | Stream          | [mailboxUsageDetail](../resources/mailboxusagedetail.md) | Erhalten Sie detaillierte Informationen über die Postfachnutzung.         |
| [Postfachanzahl abrufen](../api/reportroot-getmailboxusagemailboxcounts.md) | Stream          | [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) | Rufen Sie die Gesamtzahl der Postfächer in Ihrem Unternehmen ab und erfahren Sie, wie viele Postfächer im Berichtszeitraum täglich aktiv sind. Ein Postfach wird als aktiv betrachtet, wenn der Benutzer eine E-Mail sendet oder liest. |
| [Kontingentstatus Postfachanzahl abrufen](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | Stream          | [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) | Rufen Sie die Anzahl der Benutzerpostfächer in jeder Kontingentkategorie ab. |
| [Speicher abrufen](../api/reportroot-getmailboxusagestorage.md) | Stream          | [mailboxUsageStorage](../resources/mailboxusagestorage.md) | Erfahren Sie, wie viel Speicherplatz in Ihrer Organisation verwendet wird. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailbox-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
