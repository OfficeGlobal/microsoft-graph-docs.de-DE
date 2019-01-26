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
# <a name="mailbox-usage-reports"></a><span data-ttu-id="a20a0-104">Postfach-Verwendungsberichte</span><span class="sxs-lookup"><span data-stu-id="a20a0-104">Mailbox usage reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a20a0-105">Sie erhalten Informationen zu Benutzern mit einem Postfach und ihrer Ebene der Aktivität, die in erster Linie auf gesendeten und empfangenen e-Mails basiert.</span><span class="sxs-lookup"><span data-stu-id="a20a0-105">You can get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="a20a0-106">Sie können auch sehen, wie viel Speicherplatz jedes Postfach beansprucht und wie viele Postfächer sich den  Speicherkontingenten nähern.</span><span class="sxs-lookup"><span data-stu-id="a20a0-106">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="a20a0-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Postfachnutzung](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="a20a0-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="a20a0-108">Berichte</span><span class="sxs-lookup"><span data-stu-id="a20a0-108">Reports</span></span>

| <span data-ttu-id="a20a0-109">Function</span><span class="sxs-lookup"><span data-stu-id="a20a0-109">Function</span></span>                                 | <span data-ttu-id="a20a0-110">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="a20a0-110">CSV return type</span></span> | <span data-ttu-id="a20a0-111">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="a20a0-111">JSON return type</span></span>                         | <span data-ttu-id="a20a0-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a20a0-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="a20a0-113">Postfachdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="a20a0-113">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="a20a0-114">Stream</span><span class="sxs-lookup"><span data-stu-id="a20a0-114">Stream</span></span>          | [<span data-ttu-id="a20a0-115">mailboxUsageDetail</span><span class="sxs-lookup"><span data-stu-id="a20a0-115">mailboxUsageDetail</span></span>](../resources/mailboxusagedetail.md) | <span data-ttu-id="a20a0-116">Erhalten Sie detaillierte Informationen über die Postfachnutzung.</span><span class="sxs-lookup"><span data-stu-id="a20a0-116">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="a20a0-117">Postfachanzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="a20a0-117">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="a20a0-118">Stream</span><span class="sxs-lookup"><span data-stu-id="a20a0-118">Stream</span></span>          | [<span data-ttu-id="a20a0-119">mailboxUsageMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="a20a0-119">mailboxUsageMailboxCounts</span></span>](../resources/mailboxusagemailboxcounts.md) | <span data-ttu-id="a20a0-120">Rufen Sie die Gesamtzahl der Postfächer in Ihrem Unternehmen ab und erfahren Sie, wie viele Postfächer im Berichtszeitraum täglich aktiv sind.</span><span class="sxs-lookup"><span data-stu-id="a20a0-120">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="a20a0-121">Ein Postfach wird als aktiv betrachtet, wenn der Benutzer eine E-Mail sendet oder liest.</span><span class="sxs-lookup"><span data-stu-id="a20a0-121">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="a20a0-122">Kontingentstatus Postfachanzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="a20a0-122">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="a20a0-123">Stream</span><span class="sxs-lookup"><span data-stu-id="a20a0-123">Stream</span></span>          | [<span data-ttu-id="a20a0-124">mailboxUsageQuotaStatusMailboxCounts</span><span class="sxs-lookup"><span data-stu-id="a20a0-124">mailboxUsageQuotaStatusMailboxCounts</span></span>](../resources/mailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="a20a0-125">Rufen Sie die Anzahl der Benutzerpostfächer in jeder Kontingentkategorie ab.</span><span class="sxs-lookup"><span data-stu-id="a20a0-125">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="a20a0-126">Speicher abrufen</span><span class="sxs-lookup"><span data-stu-id="a20a0-126">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="a20a0-127">Stream</span><span class="sxs-lookup"><span data-stu-id="a20a0-127">Stream</span></span>          | [<span data-ttu-id="a20a0-128">mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="a20a0-128">mailboxUsageStorage</span></span>](../resources/mailboxusagestorage.md) | <span data-ttu-id="a20a0-129">Erfahren Sie, wie viel Speicherplatz in Ihrer Organisation verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="a20a0-129">Get the amount of storage used in your organization.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailbox-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
