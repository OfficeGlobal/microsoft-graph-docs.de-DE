---
title: SharePoint-Aktivitätsberichte
description: Sie können die Aktivität jedes Benutzers lizenziert SharePoint verwenden, anhand deren Interaktion mit Dateien abrufen. Sie können sich auch den Umfang der Zusammenarbeit basierend auf der Anzahl der freigegebenen Dateien ansehen.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 98d0393545963a73852197f5bd78241cfb958a22
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577116"
---
# <a name="sharepoint-activity-reports"></a><span data-ttu-id="eff0b-104">SharePoint-Aktivitätsberichte</span><span class="sxs-lookup"><span data-stu-id="eff0b-104">SharePoint activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eff0b-105">Sie können die Aktivität jedes Benutzers lizenziert SharePoint verwenden, anhand deren Interaktion mit Dateien abrufen.</span><span class="sxs-lookup"><span data-stu-id="eff0b-105">You can get the activity of every user licensed to use SharePoint by looking at their interaction with files.</span></span> <span data-ttu-id="eff0b-106">Sie können sich auch den Umfang der Zusammenarbeit basierend auf der Anzahl der freigegebenen Dateien ansehen.</span><span class="sxs-lookup"><span data-stu-id="eff0b-106">You can also look at the level of collaboration going on based on the number of files shared.</span></span>

> <span data-ttu-id="eff0b-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – SharePoint-Aktivität](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span><span class="sxs-lookup"><span data-stu-id="eff0b-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="reports"></a><span data-ttu-id="eff0b-108">Berichte</span><span class="sxs-lookup"><span data-stu-id="eff0b-108">Reports</span></span>

| <span data-ttu-id="eff0b-109">Function</span><span class="sxs-lookup"><span data-stu-id="eff0b-109">Function</span></span>                                 | <span data-ttu-id="eff0b-110">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="eff0b-110">CSV Return Type</span></span> | <span data-ttu-id="eff0b-111">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="eff0b-111">JSON Return Type</span></span>                         | <span data-ttu-id="eff0b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eff0b-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="eff0b-113">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="eff0b-113">Get user detail</span></span>](../api/reportroot-getsharepointactivityuserdetail.md) | <span data-ttu-id="eff0b-114">Stream</span><span class="sxs-lookup"><span data-stu-id="eff0b-114">Stream</span></span>          | [<span data-ttu-id="eff0b-115">sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="eff0b-115">sharePointActivityUserDetail</span></span>](../resources/sharepointactivityuserdetail.md) | <span data-ttu-id="eff0b-116">Rufen Sie Details zu SharePoint-Aktivitäten nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="eff0b-116">Get details about SharePoint activity by user.</span></span> |
| [<span data-ttu-id="eff0b-117">Dateianzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="eff0b-117">Get file counts</span></span>](../api/reportroot-getsharepointactivityfilecounts.md) | <span data-ttu-id="eff0b-118">Stream</span><span class="sxs-lookup"><span data-stu-id="eff0b-118">Stream</span></span>          | [<span data-ttu-id="eff0b-119">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="eff0b-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="eff0b-120">Erfahren Sie, wie viele eindeutige, lizenzierte Benutzer mit auf SharePoint-Websites gespeicherten Dateien interagiert haben.</span><span class="sxs-lookup"><span data-stu-id="eff0b-120">Get the number of unique, licensed users who interacted with files stored on SharePoint sites.</span></span> |
| [<span data-ttu-id="eff0b-121">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="eff0b-121">Get user counts</span></span>](../api/reportroot-getsharepointactivityusercounts.md) | <span data-ttu-id="eff0b-122">Stream</span><span class="sxs-lookup"><span data-stu-id="eff0b-122">Stream</span></span>          | [<span data-ttu-id="eff0b-123">sharePointActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="eff0b-123">sharePointActivityUserCounts</span></span>](../resources/sharepointactivityusercounts.md) | <span data-ttu-id="eff0b-124">Rufen Sie die Anzahl der aktiven Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="eff0b-124">Get the trend in the number of active users.</span></span> <span data-ttu-id="eff0b-125">Ein Benutzer wird als aktiv betrachtet, wenn er innerhalb des angegebenen Zeitraums eine Dateiaktivität ausgeführt (speichern, synchronisieren, ändern oder freigeben) oder eine Seite besucht hat.</span><span class="sxs-lookup"><span data-stu-id="eff0b-125">A user is considered active if he or she has executed a file activity (save, sync, modify, or share) or visited a page within the specified time period.</span></span> |
| [<span data-ttu-id="eff0b-126">Seiten abrufen</span><span class="sxs-lookup"><span data-stu-id="eff0b-126">Get pages</span></span>](../api/reportroot-getsharepointactivitypages.md) | <span data-ttu-id="eff0b-127">Stream</span><span class="sxs-lookup"><span data-stu-id="eff0b-127">Stream</span></span>          | [<span data-ttu-id="eff0b-128">sharePointActivityPages</span><span class="sxs-lookup"><span data-stu-id="eff0b-128">sharePointActivityPages</span></span>](../resources/sharepointactivitypages.md) | <span data-ttu-id="eff0b-129">Rufen Sie die Anzahl der von Benutzern besuchten eindeutigen Seiten ab.</span><span class="sxs-lookup"><span data-stu-id="eff0b-129">Get the number of unique pages visited by users.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepoint-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
