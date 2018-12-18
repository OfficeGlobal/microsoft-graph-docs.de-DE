---
title: WindowsUpdateType Enum-Typ
description: Welche Geräte Branch erhält ihre Updates aus
author: tfitzmac
ms.openlocfilehash: 415dde619529ffa9bb40ab2cea36665558bb0ee9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340838"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="ddf22-103">WindowsUpdateType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="ddf22-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="ddf22-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ddf22-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddf22-105">Welche Geräte Branch erhält ihre Updates aus</span><span class="sxs-lookup"><span data-stu-id="ddf22-105">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="ddf22-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="ddf22-106">Members</span></span>
|<span data-ttu-id="ddf22-107">Member</span><span class="sxs-lookup"><span data-stu-id="ddf22-107">Member</span></span>|<span data-ttu-id="ddf22-108">Wert</span><span class="sxs-lookup"><span data-stu-id="ddf22-108">Value</span></span>|<span data-ttu-id="ddf22-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ddf22-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddf22-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="ddf22-110">userDefined</span></span>|<span data-ttu-id="ddf22-111">0</span><span class="sxs-lookup"><span data-stu-id="ddf22-111">0</span></span>|<span data-ttu-id="ddf22-112">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="ddf22-112">Allow the user to set.</span></span>|
|<span data-ttu-id="ddf22-113">all</span><span class="sxs-lookup"><span data-stu-id="ddf22-113">all</span></span>|<span data-ttu-id="ddf22-114">1</span><span class="sxs-lookup"><span data-stu-id="ddf22-114">1</span></span>|<span data-ttu-id="ddf22-115">Semikolons jährlichen Channel (Ziel).</span><span class="sxs-lookup"><span data-stu-id="ddf22-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="ddf22-116">Gerät Ruft alle anwendbaren Feature Updates aus Semikolons jährlichen Channel (gezielte) ab.</span><span class="sxs-lookup"><span data-stu-id="ddf22-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="ddf22-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="ddf22-117">businessReadyOnly</span></span>|<span data-ttu-id="ddf22-118">2</span><span class="sxs-lookup"><span data-stu-id="ddf22-118">2</span></span>|<span data-ttu-id="ddf22-119">Semikolons jährlichen Channel.</span><span class="sxs-lookup"><span data-stu-id="ddf22-119">Semi-annual Channel.</span></span> <span data-ttu-id="ddf22-120">Gerät ruft Feature Updates aus Semikolons jährlichen Channel ab.</span><span class="sxs-lookup"><span data-stu-id="ddf22-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="ddf22-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="ddf22-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="ddf22-122">3</span><span class="sxs-lookup"><span data-stu-id="ddf22-122">3</span></span>|<span data-ttu-id="ddf22-123">Erstellen von Windows-Insider - Fast</span><span class="sxs-lookup"><span data-stu-id="ddf22-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="ddf22-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="ddf22-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="ddf22-125">4</span><span class="sxs-lookup"><span data-stu-id="ddf22-125">4</span></span>|<span data-ttu-id="ddf22-126">Erstellen von Windows-Insider - langsam</span><span class="sxs-lookup"><span data-stu-id="ddf22-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="ddf22-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="ddf22-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="ddf22-128">5</span><span class="sxs-lookup"><span data-stu-id="ddf22-128">5</span></span>|<span data-ttu-id="ddf22-129">Windows-Insider Build-Version</span><span class="sxs-lookup"><span data-stu-id="ddf22-129">Release Windows Insider build</span></span>|



