---
title: WindowsUpdateType Enum-Typ
description: Welche Geräte Branch erhält ihre Updates aus
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1444af64043ac38685ca022b56b8856be77a0b70
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944348"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="15197-103">WindowsUpdateType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="15197-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="15197-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="15197-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15197-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15197-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15197-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="15197-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15197-107">Welche Geräte Branch erhält ihre Updates aus</span><span class="sxs-lookup"><span data-stu-id="15197-107">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="15197-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="15197-108">Members</span></span>
|<span data-ttu-id="15197-109">Element</span><span class="sxs-lookup"><span data-stu-id="15197-109">Member</span></span>|<span data-ttu-id="15197-110">Wert</span><span class="sxs-lookup"><span data-stu-id="15197-110">Value</span></span>|<span data-ttu-id="15197-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15197-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15197-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="15197-112">userDefined</span></span>|<span data-ttu-id="15197-113">0</span><span class="sxs-lookup"><span data-stu-id="15197-113">0</span></span>|<span data-ttu-id="15197-114">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="15197-114">Allow the user to set.</span></span>|
|<span data-ttu-id="15197-115">all</span><span class="sxs-lookup"><span data-stu-id="15197-115">all</span></span>|<span data-ttu-id="15197-116">1</span><span class="sxs-lookup"><span data-stu-id="15197-116">1</span></span>|<span data-ttu-id="15197-117">Semikolons jährlichen Channel (Ziel).</span><span class="sxs-lookup"><span data-stu-id="15197-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="15197-118">Gerät Ruft alle anwendbaren Feature Updates aus Semikolons jährlichen Channel (gezielte) ab.</span><span class="sxs-lookup"><span data-stu-id="15197-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="15197-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="15197-119">businessReadyOnly</span></span>|<span data-ttu-id="15197-120">2</span><span class="sxs-lookup"><span data-stu-id="15197-120">2</span></span>|<span data-ttu-id="15197-121">Semikolons jährlichen Channel.</span><span class="sxs-lookup"><span data-stu-id="15197-121">Semi-annual Channel.</span></span> <span data-ttu-id="15197-122">Gerät ruft Feature Updates aus Semikolons jährlichen Channel ab.</span><span class="sxs-lookup"><span data-stu-id="15197-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="15197-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="15197-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="15197-124">3</span><span class="sxs-lookup"><span data-stu-id="15197-124">3</span></span>|<span data-ttu-id="15197-125">Erstellen von Windows-Insider - Fast</span><span class="sxs-lookup"><span data-stu-id="15197-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="15197-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="15197-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="15197-127">4</span><span class="sxs-lookup"><span data-stu-id="15197-127">4</span></span>|<span data-ttu-id="15197-128">Erstellen von Windows-Insider - langsam</span><span class="sxs-lookup"><span data-stu-id="15197-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="15197-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="15197-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="15197-130">5</span><span class="sxs-lookup"><span data-stu-id="15197-130">5</span></span>|<span data-ttu-id="15197-131">Windows-Insider Build-Version</span><span class="sxs-lookup"><span data-stu-id="15197-131">Release Windows Insider build</span></span>|





