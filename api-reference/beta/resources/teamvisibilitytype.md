---
title: Members
description: 'Beschreibt die Sichtbarkeit eines Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7e77fbd2667f8656a4c2f66046636ff73ac8891d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521348"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="daf54-103">TeamVisibilityType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="daf54-103">teamVisibilityType enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daf54-104">Beschreibt die Sichtbarkeit eines [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="daf54-104">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="daf54-105">Elemente</span><span class="sxs-lookup"><span data-stu-id="daf54-105">Members</span></span>

| <span data-ttu-id="daf54-106">Member</span><span class="sxs-lookup"><span data-stu-id="daf54-106">Member</span></span> | <span data-ttu-id="daf54-107">Wert</span><span class="sxs-lookup"><span data-stu-id="daf54-107">Value</span></span>| <span data-ttu-id="daf54-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="daf54-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="daf54-109">Private</span><span class="sxs-lookup"><span data-stu-id="daf54-109">private</span></span>|<span data-ttu-id="daf54-110">(0)</span><span class="sxs-lookup"><span data-stu-id="daf54-110">0</span></span>|<span data-ttu-id="daf54-111">Jeder Benutzer kann das Team anzeigen, aber nur der Besitzer Hinzufügen eines Benutzers an das Team.</span><span class="sxs-lookup"><span data-stu-id="daf54-111">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="daf54-112">Öffentlich</span><span class="sxs-lookup"><span data-stu-id="daf54-112">public</span></span>|<span data-ttu-id="daf54-113">-1</span><span class="sxs-lookup"><span data-stu-id="daf54-113">1</span></span>|<span data-ttu-id="daf54-114">Jeder kann das Team teilnehmen.</span><span class="sxs-lookup"><span data-stu-id="daf54-114">Anyone can join the team.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamvisibilitytype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
