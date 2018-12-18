---
title: Ressourcentyp teamMessagingSettings
description: So konfigurieren Sie die messaging-Einstellungen und erwähnungen im Team.
author: nkramer
ms.openlocfilehash: 94a102e6d0937651c990e61f4895c715b3c4bd95
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344247"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="f8901-103">Ressourcentyp teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="f8901-103">teamMessagingSettings resource type</span></span>

> <span data-ttu-id="f8901-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f8901-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8901-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8901-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8901-106">So konfigurieren Sie die messaging-Einstellungen und erwähnungen im [Team](team.md).</span><span class="sxs-lookup"><span data-stu-id="f8901-106">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f8901-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f8901-107">Properties</span></span>
| <span data-ttu-id="f8901-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8901-108">Property</span></span>     | <span data-ttu-id="f8901-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f8901-109">Type</span></span>   |<span data-ttu-id="f8901-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8901-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8901-111">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="f8901-111">allowUserEditMessages</span></span>|<span data-ttu-id="f8901-112">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f8901-112">Boolean</span></span>|<span data-ttu-id="f8901-113">Wenn es sich bei Festlegung auf true können Benutzer ihre Nachrichten bearbeiten kann.</span><span class="sxs-lookup"><span data-stu-id="f8901-113">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="f8901-114">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="f8901-114">allowUserDeleteMessages</span></span>|<span data-ttu-id="f8901-115">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f8901-115">Boolean</span></span>|<span data-ttu-id="f8901-116">Bei Festlegung auf true können Benutzer ihre Nachrichten löschen kann.</span><span class="sxs-lookup"><span data-stu-id="f8901-116">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="f8901-117">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="f8901-117">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="f8901-118">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f8901-118">Boolean</span></span>|<span data-ttu-id="f8901-119">Bei Festlegung auf "true" Websitebesitzer eine beliebige Nachricht löschen kann.</span><span class="sxs-lookup"><span data-stu-id="f8901-119">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="f8901-120">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="f8901-120">allowTeamMentions</span></span>|<span data-ttu-id="f8901-121">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f8901-121">Boolean</span></span>|<span data-ttu-id="f8901-122">Wenn Festlegung auf "true", "@team erwähnungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="f8901-122">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="f8901-123">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="f8901-123">allowChannelMentions</span></span>|<span data-ttu-id="f8901-124">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f8901-124">Boolean</span></span>|<span data-ttu-id="f8901-125">Wenn Festlegung auf "true", "@channel erwähnungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="f8901-125">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8901-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f8901-126">JSON representation</span></span>

<span data-ttu-id="f8901-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f8901-127">The following is a JSON representation of the resource.</span></span>

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
