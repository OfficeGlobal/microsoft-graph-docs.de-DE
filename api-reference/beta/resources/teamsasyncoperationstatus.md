---
title: TeamsAsyncOperationStatus Enum-Typ
description: Wird den aktuellen Status der ein TeamsAsyncOperation beschrieben.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e9138adcc646677955a12091a3fb15badfd39f13
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511709"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="172d4-103">TeamsAsyncOperationStatus Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="172d4-103">teamsAsyncOperationStatus enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="172d4-104">Wird den aktuellen Status der ein [TeamsAsyncOperation](teamsasyncoperation.md)beschrieben.</span><span class="sxs-lookup"><span data-stu-id="172d4-104">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="172d4-105">Elemente</span><span class="sxs-lookup"><span data-stu-id="172d4-105">Members</span></span>

| <span data-ttu-id="172d4-106">Member</span><span class="sxs-lookup"><span data-stu-id="172d4-106">Member</span></span> | <span data-ttu-id="172d4-107">Wert</span><span class="sxs-lookup"><span data-stu-id="172d4-107">Value</span></span>| <span data-ttu-id="172d4-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="172d4-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="172d4-109">Ungültig</span><span class="sxs-lookup"><span data-stu-id="172d4-109">invalid</span></span>|<span data-ttu-id="172d4-110">(0)</span><span class="sxs-lookup"><span data-stu-id="172d4-110">0</span></span>|<span data-ttu-id="172d4-111">Ungültiger Wert</span><span class="sxs-lookup"><span data-stu-id="172d4-111">Invalid value.</span></span>|
|<span data-ttu-id="172d4-112">NotStarted</span><span class="sxs-lookup"><span data-stu-id="172d4-112">notStarted</span></span>|<span data-ttu-id="172d4-113">-1</span><span class="sxs-lookup"><span data-stu-id="172d4-113">1</span></span>|<span data-ttu-id="172d4-114">Der Vorgang wurde nicht gestartet.</span><span class="sxs-lookup"><span data-stu-id="172d4-114">The operation has not started.</span></span>|
|<span data-ttu-id="172d4-115">InProgress</span><span class="sxs-lookup"><span data-stu-id="172d4-115">inProgress</span></span>|<span data-ttu-id="172d4-116">-2</span><span class="sxs-lookup"><span data-stu-id="172d4-116">2</span></span>|<span data-ttu-id="172d4-117">Der Vorgang wird ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="172d4-117">The operation is running.</span></span>|
|<span data-ttu-id="172d4-118">succeeded</span><span class="sxs-lookup"><span data-stu-id="172d4-118">succeeded</span></span>|<span data-ttu-id="172d4-119">-3</span><span class="sxs-lookup"><span data-stu-id="172d4-119">3</span></span>|<span data-ttu-id="172d4-120">Der Vorgang erfolgreich war.</span><span class="sxs-lookup"><span data-stu-id="172d4-120">The operation succeeded.</span></span>|
|<span data-ttu-id="172d4-121">failed</span><span class="sxs-lookup"><span data-stu-id="172d4-121">failed</span></span>|<span data-ttu-id="172d4-122">4\*</span><span class="sxs-lookup"><span data-stu-id="172d4-122">4</span></span>|<span data-ttu-id="172d4-123">Dieser Vorgang ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="172d4-123">The operation failed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
