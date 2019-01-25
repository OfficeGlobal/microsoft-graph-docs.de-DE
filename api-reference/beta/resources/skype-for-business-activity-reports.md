---
title: Skype for Business-Aktivitätsberichte
description: Sie können ausführliche Informationen zum Aktivität innerhalb Ihrer Organisation erhalten. Diese Details können Ihnen bei der Suche, Planung und Durchführung anderer Geschäftsentscheidungen innerhalb Ihrer Organisation helfen.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a81e27d58316cb415d6296b4f77519a3f2125643
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512395"
---
# <a name="skype-for-business-activity-reports"></a><span data-ttu-id="b465b-104">Skype for Business-Aktivitätsberichte</span><span class="sxs-lookup"><span data-stu-id="b465b-104">Skype for Business activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b465b-105">Sie können ausführliche Informationen zum Aktivität innerhalb Ihrer Organisation erhalten.</span><span class="sxs-lookup"><span data-stu-id="b465b-105">You can get details on activity across your organization.</span></span> <span data-ttu-id="b465b-106">Diese Details können Ihnen bei der Suche, Planung und Durchführung anderer Geschäftsentscheidungen innerhalb Ihrer Organisation helfen.</span><span class="sxs-lookup"><span data-stu-id="b465b-106">These details can help you investigate, plan, and make other business decisions for your organization.</span></span>

> <span data-ttu-id="b465b-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Aktivität](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span><span class="sxs-lookup"><span data-stu-id="b465b-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="reports"></a><span data-ttu-id="b465b-108">Berichte</span><span class="sxs-lookup"><span data-stu-id="b465b-108">Reports</span></span>

| <span data-ttu-id="b465b-109">Funktion</span><span class="sxs-lookup"><span data-stu-id="b465b-109">Function</span></span>                                 | <span data-ttu-id="b465b-110">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="b465b-110">CSV return type</span></span> | <span data-ttu-id="b465b-111">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="b465b-111">JSON return type</span></span>                         | <span data-ttu-id="b465b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b465b-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="b465b-113">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="b465b-113">Get user detail</span></span>](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | <span data-ttu-id="b465b-114">Stream</span><span class="sxs-lookup"><span data-stu-id="b465b-114">Stream</span></span>          | [<span data-ttu-id="b465b-115">skypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="b465b-115">skypeForBusinessActivityUserDetail</span></span>](../resources/skypeforbusinessactivityuserdetail.md) | <span data-ttu-id="b465b-116">Rufen Sie Details der Skype for Business-Aktivität nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="b465b-116">Get details about Skype for Business activity by user.</span></span> |
| [<span data-ttu-id="b465b-117">Aktivitätsanzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="b465b-117">Get activity counts</span></span>](../api/reportroot-getskypeforbusinessactivitycounts.md) | <span data-ttu-id="b465b-118">Stream</span><span class="sxs-lookup"><span data-stu-id="b465b-118">Stream</span></span>          | [<span data-ttu-id="b465b-119">skypeForBusinessActivityCounts</span><span class="sxs-lookup"><span data-stu-id="b465b-119">skypeForBusinessActivityCounts</span></span>](../resources/skypeforbusinessactivitycounts.md) | <span data-ttu-id="b465b-120">Rufen Sie die Trends dazu ab, wie viele Benutzer Konferenzsitzungen, die in Ihrem Unternehmen mit Skype for Business abgehalten wurden, organisiert und daran teilgenommen haben.</span><span class="sxs-lookup"><span data-stu-id="b465b-120">Get the trends on how many users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="b465b-121">Der Bericht enthält auch die Anzahl von Peer-to-Peer-Sitzungen.</span><span class="sxs-lookup"><span data-stu-id="b465b-121">The report also includes the number of peer-to-peer sessions.</span></span> |
| [<span data-ttu-id="b465b-122">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="b465b-122">Get user counts</span></span>](../api/reportroot-getskypeforbusinessactivityusercounts.md) | <span data-ttu-id="b465b-123">Stream</span><span class="sxs-lookup"><span data-stu-id="b465b-123">Stream</span></span>          | [<span data-ttu-id="b465b-124">skypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="b465b-124">skypeForBusinessActivityUserCounts</span></span>](../resources/skypeforbusinessactivityusercounts.md) | <span data-ttu-id="b465b-125">Rufen Sie die Trends dazu ab, wie viele eindeutige Benutzer Konferenzsitzungen, die in Ihrem Unternehmen mit Skype for Business abgehalten wurden, organisiert und daran teilgenommen haben.</span><span class="sxs-lookup"><span data-stu-id="b465b-125">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="b465b-126">Der Bericht enthält auch die Anzahl von Peer-to-Peer-Sitzungen.</span><span class="sxs-lookup"><span data-stu-id="b465b-126">The report also includes the number of peer-to-peer sessions.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
