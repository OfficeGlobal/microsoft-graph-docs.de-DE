---
title: ClonableTeamParts Enum-Typ
description: 'Beschreibt, welche Teil eines Teams geklont werden soll. '
localization_priority: Normal
ms.openlocfilehash: 3169d6e367484248e581c12c38887e07cf5c95af
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511464"
---
# <a name="clonableteamparts-enum-type"></a><span data-ttu-id="08f36-103">ClonableTeamParts Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="08f36-103">clonableTeamParts enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08f36-104">Beschreibt, welche Teil eines [Team](../resources/team.md) geklont werden soll.</span><span class="sxs-lookup"><span data-stu-id="08f36-104">Describes which part of a [team](../resources/team.md) should be cloned.</span></span> 

## <a name="members"></a><span data-ttu-id="08f36-105">Elemente</span><span class="sxs-lookup"><span data-stu-id="08f36-105">Members</span></span>

| <span data-ttu-id="08f36-106">Member</span><span class="sxs-lookup"><span data-stu-id="08f36-106">Member</span></span> | <span data-ttu-id="08f36-107">Wert</span><span class="sxs-lookup"><span data-stu-id="08f36-107">Value</span></span>| <span data-ttu-id="08f36-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08f36-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="08f36-109">Apps</span><span class="sxs-lookup"><span data-stu-id="08f36-109">apps</span></span>|<span data-ttu-id="08f36-110">-1</span><span class="sxs-lookup"><span data-stu-id="08f36-110">1</span></span>|<span data-ttu-id="08f36-111">Kopieren Sie die Liste der installierten apps.</span><span class="sxs-lookup"><span data-stu-id="08f36-111">Copy the list of installed apps.</span></span>|
|<span data-ttu-id="08f36-112">Registerkarten</span><span class="sxs-lookup"><span data-stu-id="08f36-112">tabs</span></span>|<span data-ttu-id="08f36-113">-2</span><span class="sxs-lookup"><span data-stu-id="08f36-113">2</span></span>|<span data-ttu-id="08f36-114">die Registerkarten in den Kanälen kopiert.</span><span class="sxs-lookup"><span data-stu-id="08f36-114">copies the tabs within channels.</span></span>|
|<span data-ttu-id="08f36-115">settings</span><span class="sxs-lookup"><span data-stu-id="08f36-115">settings</span></span>|<span data-ttu-id="08f36-116">4\*</span><span class="sxs-lookup"><span data-stu-id="08f36-116">4</span></span>|<span data-ttu-id="08f36-117">Kopiert alle Einstellungen im Team, zusammen mit den wichtigsten gruppeneinstellungen.</span><span class="sxs-lookup"><span data-stu-id="08f36-117">Copies all settings within the team, along with key group settings.</span></span>|
|<span data-ttu-id="08f36-118">Kanäle</span><span class="sxs-lookup"><span data-stu-id="08f36-118">channels</span></span>|<span data-ttu-id="08f36-119">8\*</span><span class="sxs-lookup"><span data-stu-id="08f36-119">8</span></span>|<span data-ttu-id="08f36-120">kopiert die Struktur DDE-Kanal (jedoch nicht die Nachrichten im Kanal).</span><span class="sxs-lookup"><span data-stu-id="08f36-120">copies the channel structure (but not the messages in the channel).</span></span>|
|<span data-ttu-id="08f36-121">members</span><span class="sxs-lookup"><span data-stu-id="08f36-121">members</span></span>|<span data-ttu-id="08f36-122">1.6</span><span class="sxs-lookup"><span data-stu-id="08f36-122">16</span></span>|<span data-ttu-id="08f36-123">kopiert die Elemente und Besitzer des Teams.</span><span class="sxs-lookup"><span data-stu-id="08f36-123">copies the members and owners of the team.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/clonableteamparts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
