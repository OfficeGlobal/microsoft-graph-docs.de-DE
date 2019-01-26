---
title: Microsoft Teams-Benutzeraktivitätsberichte
description: Verwenden Sie die Microsoft-Teams, Benutzerberichte, um Einblicke in die Microsoft-Teams Benutzeraktivität in Ihrer Organisation abzurufen.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 4a071fb38ce9fd76aff4ccdc648201f91a600f24
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574719"
---
# <a name="microsoft-teams-user-activity-reports"></a><span data-ttu-id="dfebe-103">Microsoft Teams-Benutzeraktivitätsberichte</span><span class="sxs-lookup"><span data-stu-id="dfebe-103">Microsoft Teams user activity reports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfebe-104">Verwenden Sie die Microsoft-Teams, Benutzerberichte, um Einblicke in die Microsoft-Teams Benutzeraktivität in Ihrer Organisation abzurufen.</span><span class="sxs-lookup"><span data-stu-id="dfebe-104">Use the Microsoft Teams user activity reports to get insights into the Microsoft Teams user activity in your organization.</span></span>

## <a name="methods"></a><span data-ttu-id="dfebe-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="dfebe-105">Methods</span></span>

| <span data-ttu-id="dfebe-106">Methode</span><span class="sxs-lookup"><span data-stu-id="dfebe-106">Method</span></span>                                   | <span data-ttu-id="dfebe-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="dfebe-107">Return Type</span></span>                              | <span data-ttu-id="dfebe-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dfebe-108">Description</span></span>                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [<span data-ttu-id="dfebe-109">Benutzerdetails abrufen</span><span class="sxs-lookup"><span data-stu-id="dfebe-109">Get user detail</span></span>](../api/reportroot-getteamsuseractivityuserdetail.md) | [<span data-ttu-id="dfebe-110">teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="dfebe-110">teamsUserActivityUserDetail</span></span>](../resources/teamsuseractivityuserdetail.md) | <span data-ttu-id="dfebe-111">Abrufen von Details zur Microsoft Teams-Benutzeraktivität nach Benutzer.</span><span class="sxs-lookup"><span data-stu-id="dfebe-111">Get details about Microsoft Teams user activity by user.</span></span> |
| [<span data-ttu-id="dfebe-112">Aktivitätsanzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="dfebe-112">Get activity counts</span></span>](../api/reportroot-getteamsuseractivitycounts.md) | [<span data-ttu-id="dfebe-113">teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="dfebe-113">teamsUserActivityCounts</span></span>](../resources/teamsuseractivitycounts.md) | <span data-ttu-id="dfebe-114">Ruft die Anzahl von Microsoft Teams-Aktivitäten nach Aktivitätstyp ab.</span><span class="sxs-lookup"><span data-stu-id="dfebe-114">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="dfebe-115">Die Aktivitätstypen geben die Anzahl von Chatnachrichten, privaten Chatnachrichten, Anrufen oder Besprechungen der Teams an.</span><span class="sxs-lookup"><span data-stu-id="dfebe-115">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
| [<span data-ttu-id="dfebe-116">Benutzeranzahl abrufen</span><span class="sxs-lookup"><span data-stu-id="dfebe-116">Get user counts</span></span>](../api/reportroot-getteamsuseractivityusercounts.md) | [<span data-ttu-id="dfebe-117">teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="dfebe-117">teamsUserActivityUserCounts</span></span>](../resources/teamsuseractivityusercounts.md) | <span data-ttu-id="dfebe-118">Ruft die Anzahl der Benutzer nach Aktivitätstyp ab.</span><span class="sxs-lookup"><span data-stu-id="dfebe-118">Get the number of users by activity type.</span></span> <span data-ttu-id="dfebe-119">Die Aktivitätstypen geben die Anzahl von Chatnachrichten, privaten Chatnachrichten, Anrufen oder Besprechungen der Teams an.</span><span class="sxs-lookup"><span data-stu-id="dfebe-119">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-user-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
