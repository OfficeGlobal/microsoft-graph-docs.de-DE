---
title: WindowsUpdateType Enum-Typ
description: Welche Geräte Branch erhält ihre Updates aus
ms.openlocfilehash: b489f17da5dc02dd7f7e72350eef282e56643dd0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019680"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="41dfc-103">WindowsUpdateType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="41dfc-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="41dfc-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="41dfc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41dfc-105">Welche Geräte Branch erhält ihre Updates aus</span><span class="sxs-lookup"><span data-stu-id="41dfc-105">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="41dfc-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="41dfc-106">Members</span></span>
|<span data-ttu-id="41dfc-107">Element</span><span class="sxs-lookup"><span data-stu-id="41dfc-107">Member</span></span>|<span data-ttu-id="41dfc-108">Wert</span><span class="sxs-lookup"><span data-stu-id="41dfc-108">Value</span></span>|<span data-ttu-id="41dfc-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41dfc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41dfc-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="41dfc-110">userDefined</span></span>|<span data-ttu-id="41dfc-111">0</span><span class="sxs-lookup"><span data-stu-id="41dfc-111">0</span></span>|<span data-ttu-id="41dfc-112">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="41dfc-112">Allow the user to set.</span></span>|
|<span data-ttu-id="41dfc-113">all</span><span class="sxs-lookup"><span data-stu-id="41dfc-113">all</span></span>|<span data-ttu-id="41dfc-114">1</span><span class="sxs-lookup"><span data-stu-id="41dfc-114">1</span></span>|<span data-ttu-id="41dfc-115">Semikolons jährlichen Channel (Ziel).</span><span class="sxs-lookup"><span data-stu-id="41dfc-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="41dfc-116">Gerät Ruft alle anwendbaren Feature Updates aus Semikolons jährlichen Channel (gezielte) ab.</span><span class="sxs-lookup"><span data-stu-id="41dfc-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="41dfc-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="41dfc-117">businessReadyOnly</span></span>|<span data-ttu-id="41dfc-118">2</span><span class="sxs-lookup"><span data-stu-id="41dfc-118">2</span></span>|<span data-ttu-id="41dfc-119">Semikolons jährlichen Channel.</span><span class="sxs-lookup"><span data-stu-id="41dfc-119">Semi-annual Channel.</span></span> <span data-ttu-id="41dfc-120">Gerät ruft Feature Updates aus Semikolons jährlichen Channel ab.</span><span class="sxs-lookup"><span data-stu-id="41dfc-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="41dfc-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="41dfc-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="41dfc-122">3</span><span class="sxs-lookup"><span data-stu-id="41dfc-122">3</span></span>|<span data-ttu-id="41dfc-123">Erstellen von Windows-Insider - Fast</span><span class="sxs-lookup"><span data-stu-id="41dfc-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="41dfc-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="41dfc-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="41dfc-125">4</span><span class="sxs-lookup"><span data-stu-id="41dfc-125">4</span></span>|<span data-ttu-id="41dfc-126">Erstellen von Windows-Insider - langsam</span><span class="sxs-lookup"><span data-stu-id="41dfc-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="41dfc-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="41dfc-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="41dfc-128">5</span><span class="sxs-lookup"><span data-stu-id="41dfc-128">5</span></span>|<span data-ttu-id="41dfc-129">Windows-Insider Build-Version</span><span class="sxs-lookup"><span data-stu-id="41dfc-129">Release Windows Insider build</span></span>|



