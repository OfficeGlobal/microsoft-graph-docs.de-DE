---
title: WindowsUpdateType Enum-Typ
description: Welche Geräte Branch erhält ihre Updates aus
author: tfitzmac
ms.openlocfilehash: b41fea0254cbbb6a590d240c2db9e4fb7aa0e6eb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309625"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="7aee4-103">WindowsUpdateType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="7aee4-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="7aee4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7aee4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7aee4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7aee4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7aee4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7aee4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7aee4-107">Welche Geräte Branch erhält ihre Updates aus</span><span class="sxs-lookup"><span data-stu-id="7aee4-107">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="7aee4-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="7aee4-108">Members</span></span>
|<span data-ttu-id="7aee4-109">Member</span><span class="sxs-lookup"><span data-stu-id="7aee4-109">Member</span></span>|<span data-ttu-id="7aee4-110">Wert</span><span class="sxs-lookup"><span data-stu-id="7aee4-110">Value</span></span>|<span data-ttu-id="7aee4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7aee4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7aee4-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="7aee4-112">userDefined</span></span>|<span data-ttu-id="7aee4-113">0</span><span class="sxs-lookup"><span data-stu-id="7aee4-113">0</span></span>|<span data-ttu-id="7aee4-114">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="7aee4-114">Allow the user to set.</span></span>|
|<span data-ttu-id="7aee4-115">all</span><span class="sxs-lookup"><span data-stu-id="7aee4-115">all</span></span>|<span data-ttu-id="7aee4-116">1</span><span class="sxs-lookup"><span data-stu-id="7aee4-116">1</span></span>|<span data-ttu-id="7aee4-117">Semikolons jährlichen Channel (Ziel).</span><span class="sxs-lookup"><span data-stu-id="7aee4-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="7aee4-118">Gerät Ruft alle anwendbaren Feature Updates aus Semikolons jährlichen Channel (gezielte) ab.</span><span class="sxs-lookup"><span data-stu-id="7aee4-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="7aee4-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="7aee4-119">businessReadyOnly</span></span>|<span data-ttu-id="7aee4-120">2</span><span class="sxs-lookup"><span data-stu-id="7aee4-120">2</span></span>|<span data-ttu-id="7aee4-121">Semikolons jährlichen Channel.</span><span class="sxs-lookup"><span data-stu-id="7aee4-121">Semi-annual Channel.</span></span> <span data-ttu-id="7aee4-122">Gerät ruft Feature Updates aus Semikolons jährlichen Channel ab.</span><span class="sxs-lookup"><span data-stu-id="7aee4-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="7aee4-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="7aee4-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="7aee4-124">3</span><span class="sxs-lookup"><span data-stu-id="7aee4-124">3</span></span>|<span data-ttu-id="7aee4-125">Erstellen von Windows-Insider - Fast</span><span class="sxs-lookup"><span data-stu-id="7aee4-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="7aee4-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="7aee4-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="7aee4-127">4</span><span class="sxs-lookup"><span data-stu-id="7aee4-127">4</span></span>|<span data-ttu-id="7aee4-128">Erstellen von Windows-Insider - langsam</span><span class="sxs-lookup"><span data-stu-id="7aee4-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="7aee4-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="7aee4-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="7aee4-130">5</span><span class="sxs-lookup"><span data-stu-id="7aee4-130">5</span></span>|<span data-ttu-id="7aee4-131">Windows-Insider Build-Version</span><span class="sxs-lookup"><span data-stu-id="7aee4-131">Release Windows Insider build</span></span>|





