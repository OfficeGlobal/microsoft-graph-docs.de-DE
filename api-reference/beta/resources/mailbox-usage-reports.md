---
title: Postfach-Verwendungsberichte
description: Sie erhalten Informationen zu Benutzern mit einem Postfach und ihrer Ebene der Aktivität, die in erster Linie auf gesendeten und empfangenen e-Mails basiert. Sie können auch sehen, wie viel Speicherplatz jedes Postfach beansprucht und wie viele Postfächer sich den  Speicherkontingenten nähern.
localization_priority: Normal
ms.openlocfilehash: 2f165ea0c9c52e1cc2f4d5fab4b8f3597fd502d3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870147"
---
# <a name="mailbox-usage-reports"></a>Postfach-Verwendungsberichte

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Sie erhalten Informationen zu Benutzern mit einem Postfach und ihrer Ebene der Aktivität, die in erster Linie auf gesendeten und empfangenen e-Mails basiert. Sie können auch sehen, wie viel Speicherplatz jedes Postfach beansprucht und wie viele Postfächer sich den  Speicherkontingenten nähern.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Postfachnutzung](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Postfachdetails abrufen](../api/reportroot-getmailboxusagedetail.md) | Stream          | [mailboxUsageDetail](../resources/mailboxusagedetail.md) | Erhalten Sie detaillierte Informationen über die Postfachnutzung.         |
| [Postfachanzahl abrufen](../api/reportroot-getmailboxusagemailboxcounts.md) | Stream          | [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) | Rufen Sie die Gesamtzahl der Postfächer in Ihrem Unternehmen ab und erfahren Sie, wie viele Postfächer im Berichtszeitraum täglich aktiv sind. Ein Postfach wird als aktiv betrachtet, wenn der Benutzer eine E-Mail sendet oder liest. |
| [Kontingentstatus Postfachanzahl abrufen](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | Stream          | [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) | Rufen Sie die Anzahl der Benutzerpostfächer in jeder Kontingentkategorie ab. |
| [Speicher abrufen](../api/reportroot-getmailboxusagestorage.md) | Stream          | [mailboxUsageStorage](../resources/mailboxusagestorage.md) | Erfahren Sie, wie viel Speicherplatz in Ihrer Organisation verwendet wird. |
