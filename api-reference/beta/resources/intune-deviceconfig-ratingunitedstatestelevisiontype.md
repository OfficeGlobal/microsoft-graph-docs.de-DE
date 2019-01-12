---
title: RatingUnitedStatesTelevisionType Enum-Typ
description: TV zum Bewerten Beschriftungen in US-Rufnummern
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9f4492fac5bc003fdaba15a39b0f58892872ea87
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964802"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="599a9-103">RatingUnitedStatesTelevisionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="599a9-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="599a9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="599a9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="599a9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="599a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="599a9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="599a9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="599a9-107">TV zum Bewerten Beschriftungen in US-Rufnummern</span><span class="sxs-lookup"><span data-stu-id="599a9-107">TV content rating labels in United States</span></span>
## <a name="members"></a><span data-ttu-id="599a9-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="599a9-108">Members</span></span>
|<span data-ttu-id="599a9-109">Element</span><span class="sxs-lookup"><span data-stu-id="599a9-109">Member</span></span>|<span data-ttu-id="599a9-110">Wert</span><span class="sxs-lookup"><span data-stu-id="599a9-110">Value</span></span>|<span data-ttu-id="599a9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="599a9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="599a9-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="599a9-112">allAllowed</span></span>|<span data-ttu-id="599a9-113">0</span><span class="sxs-lookup"><span data-stu-id="599a9-113">0</span></span>|<span data-ttu-id="599a9-114">Standardwert, zulassen, dass alle TV Inhalt anzeigt.</span><span class="sxs-lookup"><span data-stu-id="599a9-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="599a9-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="599a9-115">allBlocked</span></span>|<span data-ttu-id="599a9-116">1</span><span class="sxs-lookup"><span data-stu-id="599a9-116">1</span></span>|<span data-ttu-id="599a9-117">Lassen Sie nicht, dass alle TV Inhalt anzeigt.</span><span class="sxs-lookup"><span data-stu-id="599a9-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="599a9-118">childrenAll</span><span class="sxs-lookup"><span data-stu-id="599a9-118">childrenAll</span></span>|<span data-ttu-id="599a9-119">2</span><span class="sxs-lookup"><span data-stu-id="599a9-119">2</span></span>|<span data-ttu-id="599a9-120">TV-Y, alle untergeordneten Elemente</span><span class="sxs-lookup"><span data-stu-id="599a9-120">TV-Y, all children</span></span>|
|<span data-ttu-id="599a9-121">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="599a9-121">childrenAbove7</span></span>|<span data-ttu-id="599a9-122">3</span><span class="sxs-lookup"><span data-stu-id="599a9-122">3</span></span>|<span data-ttu-id="599a9-123">TV-Y7, untergeordnete Elemente Alter 7 und höher</span><span class="sxs-lookup"><span data-stu-id="599a9-123">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="599a9-124">Allgemeine</span><span class="sxs-lookup"><span data-stu-id="599a9-124">general</span></span>|<span data-ttu-id="599a9-125">4</span><span class="sxs-lookup"><span data-stu-id="599a9-125">4</span></span>|<span data-ttu-id="599a9-126">TV-G, für alle Jahren geeignet</span><span class="sxs-lookup"><span data-stu-id="599a9-126">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="599a9-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="599a9-127">parentalGuidance</span></span>|<span data-ttu-id="599a9-128">5</span><span class="sxs-lookup"><span data-stu-id="599a9-128">5</span></span>|<span data-ttu-id="599a9-129">TV-Seite, Eltern Anleitungen</span><span class="sxs-lookup"><span data-stu-id="599a9-129">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="599a9-130">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="599a9-130">childrenAbove14</span></span>|<span data-ttu-id="599a9-131">6</span><span class="sxs-lookup"><span data-stu-id="599a9-131">6</span></span>|<span data-ttu-id="599a9-132">TV-14, untergeordnete Elemente Alter 14 und höher</span><span class="sxs-lookup"><span data-stu-id="599a9-132">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="599a9-133">Erwachsene</span><span class="sxs-lookup"><span data-stu-id="599a9-133">adults</span></span>|<span data-ttu-id="599a9-134">7</span><span class="sxs-lookup"><span data-stu-id="599a9-134">7</span></span>|<span data-ttu-id="599a9-135">TV-MA, nur Erwachsene</span><span class="sxs-lookup"><span data-stu-id="599a9-135">TV-MA, adults only</span></span>|





