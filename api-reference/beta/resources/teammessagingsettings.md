---
title: Ressourcentyp teamMessagingSettings
description: So konfigurieren Sie die messaging-Einstellungen und erwähnungen im Team.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d98dfa3c2306cabb99b6de96aed2010cefa10717
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510099"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="aa119-103">Ressourcentyp teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="aa119-103">teamMessagingSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa119-104">So konfigurieren Sie die messaging-Einstellungen und erwähnungen im [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="aa119-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="aa119-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aa119-105">Properties</span></span>
| <span data-ttu-id="aa119-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aa119-106">Property</span></span>     | <span data-ttu-id="aa119-107">Typ</span><span class="sxs-lookup"><span data-stu-id="aa119-107">Type</span></span>   |<span data-ttu-id="aa119-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aa119-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa119-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="aa119-109">allowUserEditMessages</span></span>|<span data-ttu-id="aa119-110">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="aa119-110">Boolean</span></span>|<span data-ttu-id="aa119-111">Wenn es sich bei Festlegung auf true können Benutzer ihre Nachrichten bearbeiten kann.</span><span class="sxs-lookup"><span data-stu-id="aa119-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="aa119-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="aa119-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="aa119-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="aa119-113">Boolean</span></span>|<span data-ttu-id="aa119-114">Bei Festlegung auf true können Benutzer ihre Nachrichten löschen kann.</span><span class="sxs-lookup"><span data-stu-id="aa119-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="aa119-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="aa119-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="aa119-116">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="aa119-116">Boolean</span></span>|<span data-ttu-id="aa119-117">Bei Festlegung auf "true" Websitebesitzer eine beliebige Nachricht löschen kann.</span><span class="sxs-lookup"><span data-stu-id="aa119-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="aa119-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="aa119-118">allowTeamMentions</span></span>|<span data-ttu-id="aa119-119">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="aa119-119">Boolean</span></span>|<span data-ttu-id="aa119-120">Wenn Festlegung auf "true", "@team erwähnungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="aa119-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="aa119-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="aa119-121">allowChannelMentions</span></span>|<span data-ttu-id="aa119-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="aa119-122">Boolean</span></span>|<span data-ttu-id="aa119-123">Wenn Festlegung auf "true", "@channel erwähnungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="aa119-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa119-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aa119-124">JSON representation</span></span>

<span data-ttu-id="aa119-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aa119-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teammessagingsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
