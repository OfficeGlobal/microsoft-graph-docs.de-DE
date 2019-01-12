---
title: Ressourcentyp teamMessagingSettings
description: So konfigurieren Sie die messaging-Einstellungen und erwähnungen im Team.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 342062ee9661758c8b3179e21246b9366d832f3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930404"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="848a1-103">Ressourcentyp teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="848a1-103">teamMessagingSettings resource type</span></span>

> <span data-ttu-id="848a1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="848a1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="848a1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="848a1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="848a1-106">So konfigurieren Sie die messaging-Einstellungen und erwähnungen im [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="848a1-106">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="848a1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="848a1-107">Properties</span></span>
| <span data-ttu-id="848a1-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="848a1-108">Property</span></span>     | <span data-ttu-id="848a1-109">Typ</span><span class="sxs-lookup"><span data-stu-id="848a1-109">Type</span></span>   |<span data-ttu-id="848a1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="848a1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="848a1-111">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="848a1-111">allowUserEditMessages</span></span>|<span data-ttu-id="848a1-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="848a1-112">Boolean</span></span>|<span data-ttu-id="848a1-113">Wenn es sich bei Festlegung auf true können Benutzer ihre Nachrichten bearbeiten kann.</span><span class="sxs-lookup"><span data-stu-id="848a1-113">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="848a1-114">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="848a1-114">allowUserDeleteMessages</span></span>|<span data-ttu-id="848a1-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="848a1-115">Boolean</span></span>|<span data-ttu-id="848a1-116">Bei Festlegung auf true können Benutzer ihre Nachrichten löschen kann.</span><span class="sxs-lookup"><span data-stu-id="848a1-116">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="848a1-117">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="848a1-117">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="848a1-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="848a1-118">Boolean</span></span>|<span data-ttu-id="848a1-119">Bei Festlegung auf "true" Websitebesitzer eine beliebige Nachricht löschen kann.</span><span class="sxs-lookup"><span data-stu-id="848a1-119">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="848a1-120">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="848a1-120">allowTeamMentions</span></span>|<span data-ttu-id="848a1-121">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="848a1-121">Boolean</span></span>|<span data-ttu-id="848a1-122">Wenn Festlegung auf "true", "@team erwähnungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="848a1-122">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="848a1-123">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="848a1-123">allowChannelMentions</span></span>|<span data-ttu-id="848a1-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="848a1-124">Boolean</span></span>|<span data-ttu-id="848a1-125">Wenn Festlegung auf "true", "@channel erwähnungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="848a1-125">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="848a1-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="848a1-126">JSON representation</span></span>

<span data-ttu-id="848a1-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="848a1-127">The following is a JSON representation of the resource.</span></span>

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
