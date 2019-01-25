---
title: Yammer-Aktivitätsberichte
description: Wie viel Aktivität, über die Organisation und die Anzahl der eindeutigen Benutzer, die buchen generiert wird, like und Lesen von Nachrichten auf Yammer, können Sie die Ebene des Engagements mit Yammer Ihrer Organisation vertraut sein.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 252748b639f256467b2a01336488e1df086c69cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509938"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="2d6f9-103">Yammer-Aktivitätsberichte</span><span class="sxs-lookup"><span data-stu-id="2d6f9-103">Yammer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d6f9-104">Wie viel Aktivität, über die Organisation und die Anzahl der eindeutigen Benutzer, die buchen generiert wird, like und Lesen von Nachrichten auf Yammer, können Sie die Ebene des Engagements mit Yammer Ihrer Organisation vertraut sein.</span><span class="sxs-lookup"><span data-stu-id="2d6f9-104">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="2d6f9-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Aktivität](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="2d6f9-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="2d6f9-106">Berichte</span><span class="sxs-lookup"><span data-stu-id="2d6f9-106">Reports</span></span>

| <span data-ttu-id="2d6f9-107">Funktion</span><span class="sxs-lookup"><span data-stu-id="2d6f9-107">Function</span></span>                                 | <span data-ttu-id="2d6f9-108">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="2d6f9-108">CSV return type</span></span> | <span data-ttu-id="2d6f9-109">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="2d6f9-109">JSON return type</span></span>                         | <span data-ttu-id="2d6f9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d6f9-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="2d6f9-111">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="2d6f9-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="2d6f9-112">Stream</span><span class="sxs-lookup"><span data-stu-id="2d6f9-112">Stream</span></span>          | [<span data-ttu-id="2d6f9-113">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="2d6f9-113">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="2d6f9-114">Rufen Sie Details zu Yammer-Aktivitäten nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="2d6f9-114">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="2d6f9-115">Aktivitätsanzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="2d6f9-115">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="2d6f9-116">Stream</span><span class="sxs-lookup"><span data-stu-id="2d6f9-116">Stream</span></span>          | [<span data-ttu-id="2d6f9-117">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="2d6f9-117">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="2d6f9-118">Gewinnen Sie einen Eindruck der Yammer-Aktivitäten in Ihrer Organisation, indem Sie erfahren, wie viele Nachrichten gepostet, gelesen und gelikt wurden.</span><span class="sxs-lookup"><span data-stu-id="2d6f9-118">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="2d6f9-119">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="2d6f9-119">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="2d6f9-120">Stream</span><span class="sxs-lookup"><span data-stu-id="2d6f9-120">Stream</span></span>          | [<span data-ttu-id="2d6f9-121">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="2d6f9-121">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="2d6f9-122">Erfahren Sie, wie viele eindeutige Benutzer Yammer-Nachrichten veröffentlicht, gelesen und gelikt haben.</span><span class="sxs-lookup"><span data-stu-id="2d6f9-122">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
