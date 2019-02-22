---
title: windowsUpdateType-Enumerationstyp
description: Welche Zweigstellen-Geräte erhalten Ihre Updates von
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17aad82b25982b90ecea348d959e2ed2ec94a483
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169160"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="24903-103">windowsUpdateType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="24903-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="24903-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="24903-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24903-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="24903-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24903-106">Welche Zweigstellen-Geräte erhalten Ihre Updates von</span><span class="sxs-lookup"><span data-stu-id="24903-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="24903-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="24903-107">Members</span></span>
|<span data-ttu-id="24903-108">Element</span><span class="sxs-lookup"><span data-stu-id="24903-108">Member</span></span>|<span data-ttu-id="24903-109">Wert</span><span class="sxs-lookup"><span data-stu-id="24903-109">Value</span></span>|<span data-ttu-id="24903-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24903-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24903-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="24903-111">userDefined</span></span>|<span data-ttu-id="24903-112">0</span><span class="sxs-lookup"><span data-stu-id="24903-112">0</span></span>|<span data-ttu-id="24903-113">Zulassen, dass der Benutzer festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="24903-113">Allow the user to set.</span></span>|
|<span data-ttu-id="24903-114">all</span><span class="sxs-lookup"><span data-stu-id="24903-114">all</span></span>|<span data-ttu-id="24903-115">1</span><span class="sxs-lookup"><span data-stu-id="24903-115">1</span></span>|<span data-ttu-id="24903-116">Halbjährlicher Kanal (gezielt).</span><span class="sxs-lookup"><span data-stu-id="24903-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="24903-117">Gerät Ruft alle relevanten Feature-Updates vom halbjährlichen Kanal ab (gezielt).</span><span class="sxs-lookup"><span data-stu-id="24903-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="24903-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="24903-118">businessReadyOnly</span></span>|<span data-ttu-id="24903-119">2</span><span class="sxs-lookup"><span data-stu-id="24903-119">2</span></span>|<span data-ttu-id="24903-120">Halbjährlicher Kanal.</span><span class="sxs-lookup"><span data-stu-id="24903-120">Semi-annual Channel.</span></span> <span data-ttu-id="24903-121">Gerät ruft Feature-Updates vom halbjährlichen Kanal ab.</span><span class="sxs-lookup"><span data-stu-id="24903-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="24903-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="24903-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="24903-123">3</span><span class="sxs-lookup"><span data-stu-id="24903-123">3</span></span>|<span data-ttu-id="24903-124">Windows Insider-Erstellung – schnell</span><span class="sxs-lookup"><span data-stu-id="24903-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="24903-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="24903-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="24903-126">4</span><span class="sxs-lookup"><span data-stu-id="24903-126">4</span></span>|<span data-ttu-id="24903-127">Windows Insider Build – langsam</span><span class="sxs-lookup"><span data-stu-id="24903-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="24903-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="24903-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="24903-129">5</span><span class="sxs-lookup"><span data-stu-id="24903-129">5</span></span>|<span data-ttu-id="24903-130">Freigeben von Windows Insider Build</span><span class="sxs-lookup"><span data-stu-id="24903-130">Release Windows Insider build</span></span>|




