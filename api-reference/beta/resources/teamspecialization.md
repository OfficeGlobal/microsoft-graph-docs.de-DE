---
title: TeamSpecialization Enum-Typ
description: Beschreibt den speziellen Anwendungsfall für ein Team.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9e19c6b2242256f0d1b7a23c89aa07787bfc1913
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522651"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="12c7f-103">TeamSpecialization Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="12c7f-103">teamSpecialization enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12c7f-104">Gibt an, ob das [Team](../resources/team.md) für einen bestimmten Anwendungsfall vorgesehen ist.</span><span class="sxs-lookup"><span data-stu-id="12c7f-104">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="12c7f-105">Jedes [Team](../resources/team.md) Spezialisierung hat Zugriff zur eindeutigen Verhalten und seine Anwendungsfall Ziel Erfahrungen.</span><span class="sxs-lookup"><span data-stu-id="12c7f-105">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="12c7f-106">Standardwert ist "none".</span><span class="sxs-lookup"><span data-stu-id="12c7f-106">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="12c7f-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="12c7f-107">Members</span></span>

| <span data-ttu-id="12c7f-108">Member</span><span class="sxs-lookup"><span data-stu-id="12c7f-108">Member</span></span>             | <span data-ttu-id="12c7f-109">Wert</span><span class="sxs-lookup"><span data-stu-id="12c7f-109">Value</span></span> | <span data-ttu-id="12c7f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12c7f-110">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="12c7f-111">Keine</span><span class="sxs-lookup"><span data-stu-id="12c7f-111">none</span></span>               | <span data-ttu-id="12c7f-112">(0)</span><span class="sxs-lookup"><span data-stu-id="12c7f-112">0</span></span>     | <span data-ttu-id="12c7f-113">Standard-Typ für ein Team die die standard-Team-Erfahrung haben.</span><span class="sxs-lookup"><span data-stu-id="12c7f-113">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="12c7f-114">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="12c7f-114">unknownFutureValue</span></span> | <span data-ttu-id="12c7f-115">-7</span><span class="sxs-lookup"><span data-stu-id="12c7f-115">7</span></span>     | <span data-ttu-id="12c7f-116">Sentinel Wert als Platzhalter für zukünftige Erweiterung der Enumeration reserviert.</span><span class="sxs-lookup"><span data-stu-id="12c7f-116">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamspecialization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
