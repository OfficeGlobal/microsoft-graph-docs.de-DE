---
title: Yammer-Aktivitätsberichte
description: Wie viel Aktivität, über die Organisation und die Anzahl der eindeutigen Benutzer, die buchen generiert wird, like und Lesen von Nachrichten auf Yammer, können Sie die Ebene des Engagements mit Yammer Ihrer Organisation vertraut sein.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d5953d8bd53158b2ec0532deb47c48028ba1b8c9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571800"
---
# <a name="yammer-activity-reports"></a><span data-ttu-id="2da15-103">Yammer-Aktivitätsberichte</span><span class="sxs-lookup"><span data-stu-id="2da15-103">Yammer activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2da15-104">Wie viel Aktivität, über die Organisation und die Anzahl der eindeutigen Benutzer, die buchen generiert wird, like und Lesen von Nachrichten auf Yammer, können Sie die Ebene des Engagements mit Yammer Ihrer Organisation vertraut sein.</span><span class="sxs-lookup"><span data-stu-id="2da15-104">You can understand the level of your organization's engagement with Yammer by how much activity is generated across the organization and the number of unique users who post, like, and read messages on Yammer.</span></span>

> <span data-ttu-id="2da15-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Aktivität](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span><span class="sxs-lookup"><span data-stu-id="2da15-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="reports"></a><span data-ttu-id="2da15-106">Berichte</span><span class="sxs-lookup"><span data-stu-id="2da15-106">Reports</span></span>

| <span data-ttu-id="2da15-107">Function</span><span class="sxs-lookup"><span data-stu-id="2da15-107">Function</span></span>                                 | <span data-ttu-id="2da15-108">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="2da15-108">CSV return type</span></span> | <span data-ttu-id="2da15-109">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="2da15-109">JSON return type</span></span>                         | <span data-ttu-id="2da15-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2da15-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="2da15-111">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="2da15-111">Get user detail</span></span>](../api/reportroot-getyammeractivityuserdetail.md) | <span data-ttu-id="2da15-112">Stream</span><span class="sxs-lookup"><span data-stu-id="2da15-112">Stream</span></span>          | [<span data-ttu-id="2da15-113">yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="2da15-113">yammerActivityUserDetail</span></span>](../resources/yammeractivityuserdetail.md) | <span data-ttu-id="2da15-114">Rufen Sie Details zu Yammer-Aktivitäten nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="2da15-114">Get details about Yammer activity by user.</span></span> |
| [<span data-ttu-id="2da15-115">Aktivitätsanzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="2da15-115">Get activity counts</span></span>](../api/reportroot-getyammeractivitycounts.md) | <span data-ttu-id="2da15-116">Stream</span><span class="sxs-lookup"><span data-stu-id="2da15-116">Stream</span></span>          | [<span data-ttu-id="2da15-117">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="2da15-117">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="2da15-118">Gewinnen Sie einen Eindruck der Yammer-Aktivitäten in Ihrer Organisation, indem Sie erfahren, wie viele Nachrichten gepostet, gelesen und gelikt wurden.</span><span class="sxs-lookup"><span data-stu-id="2da15-118">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span> |
| [<span data-ttu-id="2da15-119">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="2da15-119">Get user counts</span></span>](../api/reportroot-getyammeractivityusercounts.md) | <span data-ttu-id="2da15-120">Stream</span><span class="sxs-lookup"><span data-stu-id="2da15-120">Stream</span></span>          | [<span data-ttu-id="2da15-121">yammerActivitySummary</span><span class="sxs-lookup"><span data-stu-id="2da15-121">yammerActivitySummary</span></span>](../resources/yammeractivitysummary.md) | <span data-ttu-id="2da15-122">Erfahren Sie, wie viele eindeutige Benutzer Yammer-Nachrichten veröffentlicht, gelesen und gelikt haben.</span><span class="sxs-lookup"><span data-stu-id="2da15-122">Get the trends on the number of unique users who posted, read, and liked  Yammer messages.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
