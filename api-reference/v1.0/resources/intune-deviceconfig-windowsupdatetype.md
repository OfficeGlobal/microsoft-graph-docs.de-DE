---
title: WindowsUpdateType Enum-Typ
description: Welche Geräte Branch erhält ihre Updates aus
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90d1f946dd497e650df5eb07004560dda028e14f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930341"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="cab39-103">WindowsUpdateType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="cab39-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="cab39-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cab39-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cab39-105">Welche Geräte Branch erhält ihre Updates aus</span><span class="sxs-lookup"><span data-stu-id="cab39-105">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="cab39-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="cab39-106">Members</span></span>
|<span data-ttu-id="cab39-107">Element</span><span class="sxs-lookup"><span data-stu-id="cab39-107">Member</span></span>|<span data-ttu-id="cab39-108">Wert</span><span class="sxs-lookup"><span data-stu-id="cab39-108">Value</span></span>|<span data-ttu-id="cab39-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cab39-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cab39-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="cab39-110">userDefined</span></span>|<span data-ttu-id="cab39-111">0</span><span class="sxs-lookup"><span data-stu-id="cab39-111">0</span></span>|<span data-ttu-id="cab39-112">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="cab39-112">Allow the user to set.</span></span>|
|<span data-ttu-id="cab39-113">all</span><span class="sxs-lookup"><span data-stu-id="cab39-113">all</span></span>|<span data-ttu-id="cab39-114">1</span><span class="sxs-lookup"><span data-stu-id="cab39-114">1</span></span>|<span data-ttu-id="cab39-115">Semikolons jährlichen Channel (Ziel).</span><span class="sxs-lookup"><span data-stu-id="cab39-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="cab39-116">Gerät Ruft alle anwendbaren Feature Updates aus Semikolons jährlichen Channel (gezielte) ab.</span><span class="sxs-lookup"><span data-stu-id="cab39-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="cab39-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="cab39-117">businessReadyOnly</span></span>|<span data-ttu-id="cab39-118">2</span><span class="sxs-lookup"><span data-stu-id="cab39-118">2</span></span>|<span data-ttu-id="cab39-119">Semikolons jährlichen Channel.</span><span class="sxs-lookup"><span data-stu-id="cab39-119">Semi-annual Channel.</span></span> <span data-ttu-id="cab39-120">Gerät ruft Feature Updates aus Semikolons jährlichen Channel ab.</span><span class="sxs-lookup"><span data-stu-id="cab39-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="cab39-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="cab39-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="cab39-122">3</span><span class="sxs-lookup"><span data-stu-id="cab39-122">3</span></span>|<span data-ttu-id="cab39-123">Erstellen von Windows-Insider - Fast</span><span class="sxs-lookup"><span data-stu-id="cab39-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="cab39-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="cab39-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="cab39-125">4</span><span class="sxs-lookup"><span data-stu-id="cab39-125">4</span></span>|<span data-ttu-id="cab39-126">Erstellen von Windows-Insider - langsam</span><span class="sxs-lookup"><span data-stu-id="cab39-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="cab39-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="cab39-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="cab39-128">5</span><span class="sxs-lookup"><span data-stu-id="cab39-128">5</span></span>|<span data-ttu-id="cab39-129">Windows-Insider Build-Version</span><span class="sxs-lookup"><span data-stu-id="cab39-129">Release Windows Insider build</span></span>|



