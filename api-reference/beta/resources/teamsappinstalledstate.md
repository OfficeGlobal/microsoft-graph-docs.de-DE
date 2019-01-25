---
title: Members
description: Wird den aktuelle Installationsstatus von einer TeamsApp beschrieben.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 82e46faccd2a91a82ba4fb7352391f58a42c33a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517274"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="5c416-103">TeamsAppInstalledState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="5c416-103">teamsAppInstalledState enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c416-104">Wird den aktuelle Installationsstatus von einer [TeamsApp](teamsapp.md)beschrieben.</span><span class="sxs-lookup"><span data-stu-id="5c416-104">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="5c416-105">Elemente</span><span class="sxs-lookup"><span data-stu-id="5c416-105">Members</span></span>

| <span data-ttu-id="5c416-106">Member</span><span class="sxs-lookup"><span data-stu-id="5c416-106">Member</span></span> | <span data-ttu-id="5c416-107">Wert</span><span class="sxs-lookup"><span data-stu-id="5c416-107">Value</span></span>| <span data-ttu-id="5c416-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5c416-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5c416-109">notInstalled</span><span class="sxs-lookup"><span data-stu-id="5c416-109">notInstalled</span></span>|<span data-ttu-id="5c416-110">(0)</span><span class="sxs-lookup"><span data-stu-id="5c416-110">0</span></span>|<span data-ttu-id="5c416-111">App wird an das Team nicht installiert.</span><span class="sxs-lookup"><span data-stu-id="5c416-111">App is not installed to team.</span></span>|
|<span data-ttu-id="5c416-112">Installed</span><span class="sxs-lookup"><span data-stu-id="5c416-112">installed</span></span>|<span data-ttu-id="5c416-113">-1</span><span class="sxs-lookup"><span data-stu-id="5c416-113">1</span></span>|<span data-ttu-id="5c416-114">App wird normalerweise installiert.</span><span class="sxs-lookup"><span data-stu-id="5c416-114">App is installed normally.</span></span>|
|<span data-ttu-id="5c416-115">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="5c416-115">installedAndHidden</span></span>|<span data-ttu-id="5c416-116">-2</span><span class="sxs-lookup"><span data-stu-id="5c416-116">2</span></span>|<span data-ttu-id="5c416-117">App wird installiert, jedoch ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="5c416-117">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="5c416-118">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="5c416-118">installedAndPermanent</span></span>|<span data-ttu-id="5c416-119">-3</span><span class="sxs-lookup"><span data-stu-id="5c416-119">3</span></span>|<span data-ttu-id="5c416-120">App wird dauerhaft installiert und kann nicht entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="5c416-120">App is permanently installed and may not be removed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
