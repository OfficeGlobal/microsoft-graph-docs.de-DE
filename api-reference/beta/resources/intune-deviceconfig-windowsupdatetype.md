---
title: WindowsUpdateType Enum-Typ
description: Welche Geräte Branch erhält ihre Updates aus
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 15d2d46684d38b57690cc9c12d9c49eccd652e6f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887038"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="531c0-103">WindowsUpdateType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="531c0-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="531c0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="531c0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="531c0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="531c0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="531c0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="531c0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="531c0-107">Welche Geräte Branch erhält ihre Updates aus</span><span class="sxs-lookup"><span data-stu-id="531c0-107">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="531c0-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="531c0-108">Members</span></span>
|<span data-ttu-id="531c0-109">Element</span><span class="sxs-lookup"><span data-stu-id="531c0-109">Member</span></span>|<span data-ttu-id="531c0-110">Wert</span><span class="sxs-lookup"><span data-stu-id="531c0-110">Value</span></span>|<span data-ttu-id="531c0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="531c0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="531c0-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="531c0-112">userDefined</span></span>|<span data-ttu-id="531c0-113">0</span><span class="sxs-lookup"><span data-stu-id="531c0-113">0</span></span>|<span data-ttu-id="531c0-114">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="531c0-114">Allow the user to set.</span></span>|
|<span data-ttu-id="531c0-115">all</span><span class="sxs-lookup"><span data-stu-id="531c0-115">all</span></span>|<span data-ttu-id="531c0-116">1</span><span class="sxs-lookup"><span data-stu-id="531c0-116">1</span></span>|<span data-ttu-id="531c0-117">Semikolons jährlichen Channel (Ziel).</span><span class="sxs-lookup"><span data-stu-id="531c0-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="531c0-118">Gerät Ruft alle anwendbaren Feature Updates aus Semikolons jährlichen Channel (gezielte) ab.</span><span class="sxs-lookup"><span data-stu-id="531c0-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="531c0-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="531c0-119">businessReadyOnly</span></span>|<span data-ttu-id="531c0-120">2</span><span class="sxs-lookup"><span data-stu-id="531c0-120">2</span></span>|<span data-ttu-id="531c0-121">Semikolons jährlichen Channel.</span><span class="sxs-lookup"><span data-stu-id="531c0-121">Semi-annual Channel.</span></span> <span data-ttu-id="531c0-122">Gerät ruft Feature Updates aus Semikolons jährlichen Channel ab.</span><span class="sxs-lookup"><span data-stu-id="531c0-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="531c0-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="531c0-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="531c0-124">3</span><span class="sxs-lookup"><span data-stu-id="531c0-124">3</span></span>|<span data-ttu-id="531c0-125">Erstellen von Windows-Insider - Fast</span><span class="sxs-lookup"><span data-stu-id="531c0-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="531c0-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="531c0-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="531c0-127">4</span><span class="sxs-lookup"><span data-stu-id="531c0-127">4</span></span>|<span data-ttu-id="531c0-128">Erstellen von Windows-Insider - langsam</span><span class="sxs-lookup"><span data-stu-id="531c0-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="531c0-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="531c0-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="531c0-130">5</span><span class="sxs-lookup"><span data-stu-id="531c0-130">5</span></span>|<span data-ttu-id="531c0-131">Windows-Insider Build-Version</span><span class="sxs-lookup"><span data-stu-id="531c0-131">Release Windows Insider build</span></span>|





