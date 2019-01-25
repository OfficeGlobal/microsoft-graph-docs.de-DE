---
title: Yammer-Gruppenaktivitätsberichte
description: Können Sie Einblicke in die Aktivität des Yammer-Gruppen in Ihrer Organisation erhalten und finden Sie unter wie viele Yammer-Gruppen werden erstellt und verwendet.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 05e5826a85e7d2e37af82cdf6277857746b1b922
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514159"
---
# <a name="yammer-groups-activity-reports"></a><span data-ttu-id="d2240-103">Yammer-Gruppenaktivitätsberichte</span><span class="sxs-lookup"><span data-stu-id="d2240-103">Yammer groups activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2240-104">Können Sie Einblicke in die Aktivität des Yammer-Gruppen in Ihrer Organisation erhalten und finden Sie unter wie viele Yammer-Gruppen werden erstellt und verwendet.</span><span class="sxs-lookup"><span data-stu-id="d2240-104">You can gain insights into the activity of Yammer groups in your organization and see how many Yammer groups are being created and used.</span></span>

> <span data-ttu-id="d2240-105">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gruppenaktivität](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span><span class="sxs-lookup"><span data-stu-id="d2240-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="reports"></a><span data-ttu-id="d2240-106">Berichte</span><span class="sxs-lookup"><span data-stu-id="d2240-106">Reports</span></span>

| <span data-ttu-id="d2240-107">Funktion</span><span class="sxs-lookup"><span data-stu-id="d2240-107">Function</span></span>                                 | <span data-ttu-id="d2240-108">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="d2240-108">CSV return type</span></span> | <span data-ttu-id="d2240-109">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="d2240-109">JSON return type</span></span>                         | <span data-ttu-id="d2240-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2240-110">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="d2240-111">Gruppendetails abrufen</span><span class="sxs-lookup"><span data-stu-id="d2240-111">Get group detail</span></span>](../api/reportroot-getyammergroupsactivitydetail.md) | <span data-ttu-id="d2240-112">Stream</span><span class="sxs-lookup"><span data-stu-id="d2240-112">Stream</span></span>          | [<span data-ttu-id="d2240-113">yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="d2240-113">yammerGroupsActivityDetail</span></span>](../resources/yammergroupsactivitydetail.md) | <span data-ttu-id="d2240-114">Rufen Sie Details zur Yammer-Gruppenaktivität nach Gruppe ab.</span><span class="sxs-lookup"><span data-stu-id="d2240-114">Get details about Yammer groups activity by group.</span></span> |
| [<span data-ttu-id="d2240-115">Gruppenanzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="d2240-115">Get group counts</span></span>](../api/reportroot-getyammergroupsactivitygroupcounts.md) | <span data-ttu-id="d2240-116">Stream</span><span class="sxs-lookup"><span data-stu-id="d2240-116">Stream</span></span>          | [<span data-ttu-id="d2240-117">yammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="d2240-117">yammerGroupsActivityGroupCounts</span></span>](../resources/yammergroupsactivitygroupcounts.md) | <span data-ttu-id="d2240-118">Erfahren Sie, wie viele Gruppen bisher vorhanden waren und bei wie vielen davon Gruppenunterhaltungsaktivitäten ausgeführt wurden.</span><span class="sxs-lookup"><span data-stu-id="d2240-118">Get the total number of groups that existed and how many included group conversation activity.</span></span> |
| [<span data-ttu-id="d2240-119">Aktivitätsanzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="d2240-119">Get activity counts</span></span>](../api/reportroot-getyammergroupsactivitycounts.md) | <span data-ttu-id="d2240-120">Stream</span><span class="sxs-lookup"><span data-stu-id="d2240-120">Stream</span></span>          | [<span data-ttu-id="d2240-121">yammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="d2240-121">yammerGroupsActivityCounts</span></span>](../resources/yammergroupsactivitycounts.md) | <span data-ttu-id="d2240-122">Rufen Sie die Anzahl der in Gruppen veröffentlichten, gelesenen und gelikten Yammer-Nachrichten ab.</span><span class="sxs-lookup"><span data-stu-id="d2240-122">Get the number of Yammer messages posted, read, and liked in groups.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-groups-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
