---
title: Postfach-Verwendungsberichte
description: Nutzen Sie die Postfach-Verwendungsberichte, um Informationen zu Benutzern mit einem Postfach und deren Aktivitätsniveau, das hauptsächlich auf gesendeten und empfangenen E-Mails basiert, zu erhalten. Sie können auch sehen, wie viel Speicherplatz jedes Postfach beansprucht und wie viele Postfächer sich den  Speicherkontingenten nähern.
ms.openlocfilehash: 6ebaa1e829d4f97f8fa354a42a175a8f392e0c69
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018272"
---
# <a name="mailbox-usage-reports"></a><span data-ttu-id="a091f-104">Postfach-Verwendungsberichte</span><span class="sxs-lookup"><span data-stu-id="a091f-104">Mailbox usage reports</span></span>

<span data-ttu-id="a091f-105">Nutzen Sie die Postfach-Verwendungsberichte, um Informationen zu Benutzern mit einem Postfach und deren Aktivitätsniveau, das hauptsächlich auf gesendeten und empfangenen E-Mails basiert, zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="a091f-105">Use the mailbox usage reports to get information about users with a mailbox and their level of activity which is primarily based on emails sent and received.</span></span> <span data-ttu-id="a091f-106">Sie können auch sehen, wie viel Speicherplatz jedes Postfach beansprucht und wie viele Postfächer sich den  Speicherkontingenten nähern.</span><span class="sxs-lookup"><span data-stu-id="a091f-106">You can also see how much storage each mailbox consumes and how many mailboxes are approaching storage quotas.</span></span>

> <span data-ttu-id="a091f-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Postfachnutzung](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span><span class="sxs-lookup"><span data-stu-id="a091f-107">**Note:** For details about different report views and names, see [Office 365 Reports - Mailbox usage](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729).</span></span>

## <a name="reports"></a><span data-ttu-id="a091f-108">Berichte</span><span class="sxs-lookup"><span data-stu-id="a091f-108">Reports</span></span>

| <span data-ttu-id="a091f-109">Funktion</span><span class="sxs-lookup"><span data-stu-id="a091f-109">Function</span></span>                                 | <span data-ttu-id="a091f-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a091f-110">Return Type</span></span> | <span data-ttu-id="a091f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a091f-111">Description</span></span>                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [<span data-ttu-id="a091f-112">Postfachdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="a091f-112">Get mailbox detail</span></span>](../api/reportroot-getmailboxusagedetail.md) | <span data-ttu-id="a091f-113">Stream</span><span class="sxs-lookup"><span data-stu-id="a091f-113">Stream</span></span>      | <span data-ttu-id="a091f-114">Erhalten Sie detaillierte Informationen über die Postfachnutzung.</span><span class="sxs-lookup"><span data-stu-id="a091f-114">Get details about mailbox usage.</span></span>         |
| [<span data-ttu-id="a091f-115">Postfachanzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="a091f-115">Get mailbox counts</span></span>](../api/reportroot-getmailboxusagemailboxcounts.md) | <span data-ttu-id="a091f-116">Stream</span><span class="sxs-lookup"><span data-stu-id="a091f-116">Stream</span></span>      | <span data-ttu-id="a091f-117">Rufen Sie die Gesamtzahl der Postfächer in Ihrem Unternehmen ab und erfahren Sie, wie viele Postfächer im Berichtszeitraum täglich aktiv sind.</span><span class="sxs-lookup"><span data-stu-id="a091f-117">Get the total number of user mailboxes in your organization and how many are active each day of the reporting period.</span></span> <span data-ttu-id="a091f-118">Ein Postfach wird als aktiv betrachtet, wenn der Benutzer eine E-Mail sendet oder liest.</span><span class="sxs-lookup"><span data-stu-id="a091f-118">A mailbox is considered active if the user sent or read any email.</span></span> |
| [<span data-ttu-id="a091f-119">Kontingentstatus Postfachanzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="a091f-119">Get quota status mailbox counts</span></span>](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md) | <span data-ttu-id="a091f-120">Stream</span><span class="sxs-lookup"><span data-stu-id="a091f-120">Stream</span></span>      | <span data-ttu-id="a091f-121">Rufen Sie die Anzahl der Benutzerpostfächer in jeder Kontingentkategorie ab.</span><span class="sxs-lookup"><span data-stu-id="a091f-121">Get the count of user mailboxes in each quota category.</span></span> |
| [<span data-ttu-id="a091f-122">Speicher abrufen</span><span class="sxs-lookup"><span data-stu-id="a091f-122">Get storage</span></span>](../api/reportroot-getmailboxusagestorage.md) | <span data-ttu-id="a091f-123">Stream</span><span class="sxs-lookup"><span data-stu-id="a091f-123">Stream</span></span>      | <span data-ttu-id="a091f-124">Erfahren Sie, wie viel Speicherplatz in Ihrer Organisation verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="a091f-124">Get the amount of storage used in your organization.</span></span> |