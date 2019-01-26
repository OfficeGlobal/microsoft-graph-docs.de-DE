---
title: Skype for Business-Aktivitätsberichte
description: Sie können ausführliche Informationen zum Aktivität innerhalb Ihrer Organisation erhalten. Diese Details können Ihnen bei der Suche, Planung und Durchführung anderer Geschäftsentscheidungen innerhalb Ihrer Organisation helfen.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 3f843efc6834ee59872e7bf750174558cdb0a103
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577382"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="778ac-104">Skype for Business-Aktivitätsberichte</span><span class="sxs-lookup"><span data-stu-id="778ac-104">Skype for Business activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="778ac-105">Sie können ausführliche Informationen zum Aktivität innerhalb Ihrer Organisation erhalten.</span><span class="sxs-lookup"><span data-stu-id="778ac-105">You can get details on activity across your organization.</span></span> <span data-ttu-id="778ac-106">Diese Details können Ihnen bei der Suche, Planung und Durchführung anderer Geschäftsentscheidungen innerhalb Ihrer Organisation helfen.</span><span class="sxs-lookup"><span data-stu-id="778ac-106">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="778ac-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Aktivität](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="778ac-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="778ac-108">Berichte</span><span class="sxs-lookup"><span data-stu-id="778ac-108">Reports</span></span>

| <span data-ttu-id="778ac-109">Function</span><span class="sxs-lookup"><span data-stu-id="778ac-109">Function</span></span>                                 | <span data-ttu-id="778ac-110">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="778ac-110">CSV return type</span></span> | <span data-ttu-id="778ac-111">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="778ac-111">JSON return type</span></span>                         | <span data-ttu-id="778ac-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="778ac-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="778ac-113">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="778ac-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="778ac-114">Stream</span><span class="sxs-lookup"><span data-stu-id="778ac-114">Stream</span></span>          | [<span data-ttu-id="778ac-115">skypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="778ac-115">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="778ac-116">Rufen Sie Details der Skype for Business-Aktivität nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="778ac-116">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="778ac-117">Aktivitätsanzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="778ac-117">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="778ac-118">Stream</span><span class="sxs-lookup"><span data-stu-id="778ac-118">Stream</span></span>          | [<span data-ttu-id="778ac-119">skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="778ac-119">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="778ac-120">Rufen Sie die Trends dazu ab, wie viele Benutzer Konferenzsitzungen, die in Ihrem Unternehmen mit Skype for Business abgehalten wurden, organisiert und daran teilgenommen haben.</span><span class="sxs-lookup"><span data-stu-id="778ac-120">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="778ac-121">Der Bericht enthält auch die Anzahl von Peer-to-Peer-Sitzungen.</span><span class="sxs-lookup"><span data-stu-id="778ac-121">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="778ac-122">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="778ac-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="778ac-123">Stream</span><span class="sxs-lookup"><span data-stu-id="778ac-123">Stream</span></span>          | [<span data-ttu-id="778ac-124">skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="778ac-124">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="778ac-125">Rufen Sie die Trends dazu ab, wie viele eindeutige Benutzer Konferenzsitzungen, die in Ihrem Unternehmen mit Skype for Business abgehalten wurden, organisiert und daran teilgenommen haben.</span><span class="sxs-lookup"><span data-stu-id="778ac-125">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="778ac-126">Der Bericht enthält auch die Anzahl von Peer-to-Peer-Sitzungen.</span><span class="sxs-lookup"><span data-stu-id="778ac-126">The report also includes the number of peer-to-peer sessions.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
