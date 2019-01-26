---
title: OneDrive-Aktivitätsberichte
description: Sie können die Aktivität jedes Benutzers OneDrive verwenden, indem Sie deren Interaktion mit Dateien auf OneDrive betrachten lizenziert abrufen. Außerdem können Sie zu verstehen, die Ebene der Zusammenarbeit wie folgt die Anzahl der freigegebenen Dateien fortfahren.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d545f1d92beee89e19eb47cfd8c6ba8c391c5349
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574005"
---
# <a name="onedrive-activity-reports"></a><span data-ttu-id="6fe20-104">OneDrive-Aktivitätsberichte</span><span class="sxs-lookup"><span data-stu-id="6fe20-104">OneDrive activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fe20-105">Sie können die Aktivität jedes Benutzers OneDrive verwenden, indem Sie deren Interaktion mit Dateien auf OneDrive betrachten lizenziert abrufen.</span><span class="sxs-lookup"><span data-stu-id="6fe20-105">You can get the activity of every user licensed to use OneDrive by looking at their interaction with files on OneDrive.</span></span> <span data-ttu-id="6fe20-106">Außerdem können Sie zu verstehen, die Ebene der Zusammenarbeit wie folgt die Anzahl der freigegebenen Dateien fortfahren.</span><span class="sxs-lookup"><span data-stu-id="6fe20-106">It also helps you to understand the level of collaboration going on by showing the number of files shared.</span></span>

> <span data-ttu-id="6fe20-107">**Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – OneDrive for Business-Aktivität](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span><span class="sxs-lookup"><span data-stu-id="6fe20-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="reports"></a><span data-ttu-id="6fe20-108">Berichte</span><span class="sxs-lookup"><span data-stu-id="6fe20-108">Reports</span></span>

| <span data-ttu-id="6fe20-109">Function</span><span class="sxs-lookup"><span data-stu-id="6fe20-109">Function</span></span>                                 | <span data-ttu-id="6fe20-110">Rückgabetyp CSV</span><span class="sxs-lookup"><span data-stu-id="6fe20-110">CSV return type</span></span> | <span data-ttu-id="6fe20-111">Rückgabetyp JSON</span><span class="sxs-lookup"><span data-stu-id="6fe20-111">JSON return type</span></span>                         | <span data-ttu-id="6fe20-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6fe20-112">Description</span></span>                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [<span data-ttu-id="6fe20-113">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="6fe20-113">Get user detail</span></span>](../api/reportroot-getonedriveactivityuserdetail.md) | <span data-ttu-id="6fe20-114">Stream</span><span class="sxs-lookup"><span data-stu-id="6fe20-114">Stream</span></span>          | [<span data-ttu-id="6fe20-115">oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="6fe20-115">oneDriveActivityUserDetail</span></span>](../resources/onedriveactivityuserdetail.md) | <span data-ttu-id="6fe20-116">Rufen Sie Details zu OneDrive-Aktivitäten nach Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="6fe20-116">Get details about OneDrive activity by user.</span></span> |
| [<span data-ttu-id="6fe20-117">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="6fe20-117">Get user counts</span></span>](../api/reportroot-getonedriveactivityusercounts.md) | <span data-ttu-id="6fe20-118">Stream</span><span class="sxs-lookup"><span data-stu-id="6fe20-118">Stream</span></span>          | [<span data-ttu-id="6fe20-119">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="6fe20-119">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="6fe20-120">Rufen Sie die Anzahl der aktiven OneDrive-Benutzer ab.</span><span class="sxs-lookup"><span data-stu-id="6fe20-120">Get the trend in the number of active OneDrive users.</span></span> |
| [<span data-ttu-id="6fe20-121">Dateianzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="6fe20-121">Get file counts</span></span>](../api/reportroot-getonedriveactivityfilecounts.md) | <span data-ttu-id="6fe20-122">Stream</span><span class="sxs-lookup"><span data-stu-id="6fe20-122">Stream</span></span>          | [<span data-ttu-id="6fe20-123">siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="6fe20-123">siteActivitySummary</span></span>](../resources/siteactivitysummary.md) | <span data-ttu-id="6fe20-124">Rufen Sie die Anzahl der eindeutigen, lizenzierten Benutzer ab, die Dateiinteraktionen für beliebige OneDrive-Konten ausgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="6fe20-124">Get the number of unique, licensed users that performed file interactions against any OneDrive account.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onedrive-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
