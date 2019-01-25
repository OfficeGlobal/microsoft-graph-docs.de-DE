---
title: SharePoint-Aktivitätsberichte
description: Sie können die Aktivität jedes Benutzers lizenziert SharePoint verwenden, anhand deren Interaktion mit Dateien abrufen. Sie können sich auch den Umfang der Zusammenarbeit basierend auf der Anzahl der freigegebenen Dateien ansehen.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 55013b3ada74e876734a83acf512a532e32cc4be
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522196"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="0e680-104">SharePoint-Aktivitätsberichte</span><span class="sxs-lookup"><span data-stu-id="0e680-104">SharePoint activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e680-105">Sie können die Aktivität jedes Benutzers lizenziert SharePoint verwenden, anhand deren Interaktion mit Dateien abrufen.</span><span class="sxs-lookup"><span data-stu-id="0e680-105">You can get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="0e680-106">Sie können sich auch den Umfang der Zusammenarbeit basierend auf der Anzahl der freigegebenen Dateien ansehen.</span><span class="sxs-lookup"><span data-stu-id="0e680-106">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="0e680-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Aktivität](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="0e680-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="0e680-108">Berichte</span><span class="sxs-lookup"><span data-stu-id="0e680-108">Reports</span></span>

| <span data-ttu-id="0e680-109">Funktion</span><span class="sxs-lookup"><span data-stu-id="0e680-109">Function</span></span>                                 | <span data-ttu-id="0e680-110">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="0e680-110">CSV Return Type</span></span> | <span data-ttu-id="0e680-111">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="0e680-111">JSON Return Type</span></span>                         | <span data-ttu-id="0e680-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e680-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="0e680-113">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="0e680-113">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="0e680-114">Stream</span><span class="sxs-lookup"><span data-stu-id="0e680-114">Stream</span></span>          | [<span data-ttu-id="0e680-115">sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="0e680-115">sharePointActivityUserDetail</span></span>](../resources/sharepointactivityuserdetail.md) | <span data-ttu-id="0e680-116">Rufen Sie Details zu SharePoint-Aktivitäten nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="0e680-116">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="0e680-117">Dateianzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="0e680-117">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="0e680-118">Stream</span><span class="sxs-lookup"><span data-stu-id="0e680-118">Stream</span></span>          | [<span data-ttu-id="0e680-119">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="0e680-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="0e680-120">Erfahren Sie, wie viele eindeutige, lizenzierte Benutzer mit auf SharePoint-Websites gespeicherten Dateien interagiert haben.</span><span class="sxs-lookup"><span data-stu-id="0e680-120">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="0e680-121">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="0e680-121">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="0e680-122">Stream</span><span class="sxs-lookup"><span data-stu-id="0e680-122">Stream</span></span>          | [<span data-ttu-id="0e680-123">sharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="0e680-123">sharePointActivityUserCounts</span></span>](../resources/sharepointactivityusercounts.md) | <span data-ttu-id="0e680-124">Rufen Sie die Anzahl der aktiven Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="0e680-124">Get the trend in the number of active users.</span></span> <span data-ttu-id="0e680-125">Ein Benutzer wird als aktiv betrachtet, wenn er innerhalb des angegebenen Zeitraums eine Dateiaktivität ausgeführt (speichern, synchronisieren, ändern oder freigeben) oder eine Seite besucht hat.</span><span class="sxs-lookup"><span data-stu-id="0e680-125">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="0e680-126">Seiten abrufen</span><span class="sxs-lookup"><span data-stu-id="0e680-126">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="0e680-127">Stream</span><span class="sxs-lookup"><span data-stu-id="0e680-127">Stream</span></span>          | [<span data-ttu-id="0e680-128">sharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="0e680-128">sharePointActivityPages</span></span>](../resources/sharepointactivitypages.md) | <span data-ttu-id="0e680-129">Rufen Sie die Anzahl der von Benutzern besuchten eindeutigen Seiten ab.</span><span class="sxs-lookup"><span data-stu-id="0e680-129">Get the number of unique pages visited by users.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepoint-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
