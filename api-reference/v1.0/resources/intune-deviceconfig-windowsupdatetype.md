---
title: windowsUpdateType-Enumerationstyp
description: Welche Zweigstellen-Geräte erhalten Ihre Updates von
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f91657cabec59cf1307253d707ba632bf4f99463
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260221"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="48327-103">windowsUpdateType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="48327-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="48327-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="48327-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48327-105">Welche Zweigstellen-Geräte erhalten Ihre Updates von</span><span class="sxs-lookup"><span data-stu-id="48327-105">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="48327-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="48327-106">Members</span></span>
|<span data-ttu-id="48327-107">Element</span><span class="sxs-lookup"><span data-stu-id="48327-107">Member</span></span>|<span data-ttu-id="48327-108">Wert</span><span class="sxs-lookup"><span data-stu-id="48327-108">Value</span></span>|<span data-ttu-id="48327-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48327-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48327-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="48327-110">userDefined</span></span>|<span data-ttu-id="48327-111">0</span><span class="sxs-lookup"><span data-stu-id="48327-111">0</span></span>|<span data-ttu-id="48327-112">Zulassen, dass der Benutzer festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="48327-112">Allow the user to set.</span></span>|
|<span data-ttu-id="48327-113">all</span><span class="sxs-lookup"><span data-stu-id="48327-113">all</span></span>|<span data-ttu-id="48327-114">1</span><span class="sxs-lookup"><span data-stu-id="48327-114">1</span></span>|<span data-ttu-id="48327-115">Halbjährlicher Kanal (gezielt).</span><span class="sxs-lookup"><span data-stu-id="48327-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="48327-116">Gerät Ruft alle relevanten Feature-Updates vom halbjährlichen Kanal ab (gezielt).</span><span class="sxs-lookup"><span data-stu-id="48327-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="48327-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="48327-117">businessReadyOnly</span></span>|<span data-ttu-id="48327-118">2</span><span class="sxs-lookup"><span data-stu-id="48327-118">2</span></span>|<span data-ttu-id="48327-119">Halbjährlicher Kanal.</span><span class="sxs-lookup"><span data-stu-id="48327-119">Semi-annual Channel.</span></span> <span data-ttu-id="48327-120">Gerät ruft Feature-Updates vom halbjährlichen Kanal ab.</span><span class="sxs-lookup"><span data-stu-id="48327-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="48327-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="48327-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="48327-122">3</span><span class="sxs-lookup"><span data-stu-id="48327-122">3</span></span>|<span data-ttu-id="48327-123">Windows Insider-Erstellung – schnell</span><span class="sxs-lookup"><span data-stu-id="48327-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="48327-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="48327-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="48327-125">4</span><span class="sxs-lookup"><span data-stu-id="48327-125">4</span></span>|<span data-ttu-id="48327-126">Windows Insider Build – langsam</span><span class="sxs-lookup"><span data-stu-id="48327-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="48327-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="48327-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="48327-128">5</span><span class="sxs-lookup"><span data-stu-id="48327-128">5</span></span>|<span data-ttu-id="48327-129">Freigeben von Windows Insider Build</span><span class="sxs-lookup"><span data-stu-id="48327-129">Release Windows Insider build</span></span>|



