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
# <a name="email-activity-reports"></a><span data-ttu-id="6466f-104">E-Mail-Aktivitätsberichte</span><span class="sxs-lookup"><span data-stu-id="6466f-104">Email activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6466f-105">Sie können eine Ansicht der e-Mail-Verkehr auf oberster Ebene innerhalb Ihrer Organisation über die Seite Berichte abrufen.</span><span class="sxs-lookup"><span data-stu-id="6466f-105">You can get a high level view of email traffic within your organization from the Reports page.</span></span> <span data-ttu-id="6466f-106">Sie können auch in der e-Mail-Aktivität-Widget zu verstehen, die Trends und Details pro Benutzer, der die e-Mail-Aktivität in Ihrer Organisation anzeigen.</span><span class="sxs-lookup"><span data-stu-id="6466f-106">You can also drill into the Email Activity widget to understand the trends and details per user of the email activity in your organization.</span></span>

> <span data-ttu-id="6466f-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – E-Mail-Aktivität](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span><span class="sxs-lookup"><span data-stu-id="6466f-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="reports"></a><span data-ttu-id="6466f-108">Berichte</span><span class="sxs-lookup"><span data-stu-id="6466f-108">Reports</span></span>

| <span data-ttu-id="6466f-109">Function</span><span class="sxs-lookup"><span data-stu-id="6466f-109">Function</span></span>                                 | <span data-ttu-id="6466f-110">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="6466f-110">CSV return type</span></span> | <span data-ttu-id="6466f-111">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="6466f-111">JSON return type</span></span>                         | <span data-ttu-id="6466f-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6466f-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="6466f-113">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="6466f-113">Get user detail</span></span>](../api/reportroot-getemailactivityuserdetail.md) | <span data-ttu-id="6466f-114">Stream</span><span class="sxs-lookup"><span data-stu-id="6466f-114">Stream</span></span>          | [<span data-ttu-id="6466f-115">emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="6466f-115">emailActivityUserDetail</span></span>](../resources/emailactivityuserdetail.md) | <span data-ttu-id="6466f-116">Erhalten Sie detaillierte Informationen über die von Benutzern ausgeführten E-Mail-Aktivitäten.</span><span class="sxs-lookup"><span data-stu-id="6466f-116">Get details about email activity users have performed.</span></span> |
| [<span data-ttu-id="6466f-117">Aktivitätsanzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="6466f-117">Get activity counts</span></span>](../api/reportroot-getemailactivitycounts.md) | <span data-ttu-id="6466f-118">Stream</span><span class="sxs-lookup"><span data-stu-id="6466f-118">Stream</span></span>          | [<span data-ttu-id="6466f-119">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="6466f-119">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="6466f-120">Ermöglicht es Ihnen, einen Überblick über die E-Mail-Aktivitäten (z. B. wie viele E-Mails versendet, gelesen und empfangen wurden) in Ihrer Organisation zu gewinnen.</span><span class="sxs-lookup"><span data-stu-id="6466f-120">Enables you to understand the trends of email activity (like how many were sent, read, and received) in your organization.</span></span> |
| [<span data-ttu-id="6466f-121">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="6466f-121">Get user counts</span></span>](../api/reportroot-getemailactivityusercounts.md) | <span data-ttu-id="6466f-122">Stream</span><span class="sxs-lookup"><span data-stu-id="6466f-122">Stream</span></span>          | [<span data-ttu-id="6466f-123">emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="6466f-123">emailActivitySummary</span></span>](../resources/emailactivitysummary.md) | <span data-ttu-id="6466f-124">Ermöglicht es Ihnen, sich anhand der Anzahl eindeutiger Benutzer, die E-Mail-Aktivitäten wie Senden, Lesen und Empfangen ausführen, über Trends zu informieren.</span><span class="sxs-lookup"><span data-stu-id="6466f-124">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/email-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
