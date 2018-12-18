---
title: Ressourcentyp teamMessagingSettings
description: So konfigurieren Sie die messaging-Einstellungen und erwähnungen im Team.
author: nkramer
ms.openlocfilehash: 387c2e3ccedc6f11f17d4868b1b0d3eaf67624fa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304550"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="7176d-103">Ressourcentyp teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="7176d-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="7176d-104">So konfigurieren Sie die messaging-Einstellungen und erwähnungen im [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="7176d-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7176d-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7176d-105">Properties</span></span>
| <span data-ttu-id="7176d-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7176d-106">Property</span></span>     | <span data-ttu-id="7176d-107">Typ</span><span class="sxs-lookup"><span data-stu-id="7176d-107">Type</span></span>   |<span data-ttu-id="7176d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7176d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7176d-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="7176d-109">allowUserEditMessages</span></span>|<span data-ttu-id="7176d-110">Boolesch</span><span class="sxs-lookup"><span data-stu-id="7176d-110">Boolean</span></span>|<span data-ttu-id="7176d-111">Wenn es sich bei Festlegung auf true können Benutzer ihre Nachrichten bearbeiten kann.</span><span class="sxs-lookup"><span data-stu-id="7176d-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="7176d-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="7176d-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="7176d-113">Boolesch</span><span class="sxs-lookup"><span data-stu-id="7176d-113">Boolean</span></span>|<span data-ttu-id="7176d-114">Bei Festlegung auf true können Benutzer ihre Nachrichten löschen kann.</span><span class="sxs-lookup"><span data-stu-id="7176d-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="7176d-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="7176d-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="7176d-116">Boolesch</span><span class="sxs-lookup"><span data-stu-id="7176d-116">Boolean</span></span>|<span data-ttu-id="7176d-117">Bei Festlegung auf "true" Websitebesitzer eine beliebige Nachricht löschen kann.</span><span class="sxs-lookup"><span data-stu-id="7176d-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="7176d-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="7176d-118">allowTeamMentions</span></span>|<span data-ttu-id="7176d-119">Boolesch</span><span class="sxs-lookup"><span data-stu-id="7176d-119">Boolean</span></span>|<span data-ttu-id="7176d-120">Wenn Festlegung auf "true", "@team erwähnungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="7176d-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="7176d-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="7176d-121">allowChannelMentions</span></span>|<span data-ttu-id="7176d-122">Boolesch</span><span class="sxs-lookup"><span data-stu-id="7176d-122">Boolean</span></span>|<span data-ttu-id="7176d-123">Wenn Festlegung auf "true", "@channel erwähnungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="7176d-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7176d-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7176d-124">JSON representation</span></span>

<span data-ttu-id="7176d-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7176d-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
