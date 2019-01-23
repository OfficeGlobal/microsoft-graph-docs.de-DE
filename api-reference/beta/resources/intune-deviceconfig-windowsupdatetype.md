---
title: WindowsUpdateType Enum-Typ
description: Welche Geräte Branch erhält ihre Updates aus
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d3dd0f6d8ba46d7f1cc803b217a98a862602149
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400137"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="1fcc0-103">WindowsUpdateType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="1fcc0-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="1fcc0-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1fcc0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1fcc0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fcc0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1fcc0-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1fcc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fcc0-107">Welche Geräte Branch erhält ihre Updates aus</span><span class="sxs-lookup"><span data-stu-id="1fcc0-107">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="1fcc0-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="1fcc0-108">Members</span></span>
|<span data-ttu-id="1fcc0-109">Member</span><span class="sxs-lookup"><span data-stu-id="1fcc0-109">Member</span></span>|<span data-ttu-id="1fcc0-110">Wert</span><span class="sxs-lookup"><span data-stu-id="1fcc0-110">Value</span></span>|<span data-ttu-id="1fcc0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1fcc0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fcc0-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="1fcc0-112">userDefined</span></span>|<span data-ttu-id="1fcc0-113">0</span><span class="sxs-lookup"><span data-stu-id="1fcc0-113">0</span></span>|<span data-ttu-id="1fcc0-114">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="1fcc0-114">Allow the user to set.</span></span>|
|<span data-ttu-id="1fcc0-115">all</span><span class="sxs-lookup"><span data-stu-id="1fcc0-115">all</span></span>|<span data-ttu-id="1fcc0-116">1</span><span class="sxs-lookup"><span data-stu-id="1fcc0-116">1</span></span>|<span data-ttu-id="1fcc0-117">Semikolons jährlichen Channel (Ziel).</span><span class="sxs-lookup"><span data-stu-id="1fcc0-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="1fcc0-118">Gerät Ruft alle anwendbaren Feature Updates aus Semikolons jährlichen Channel (gezielte) ab.</span><span class="sxs-lookup"><span data-stu-id="1fcc0-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="1fcc0-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="1fcc0-119">businessReadyOnly</span></span>|<span data-ttu-id="1fcc0-120">2</span><span class="sxs-lookup"><span data-stu-id="1fcc0-120">2</span></span>|<span data-ttu-id="1fcc0-121">Semikolons jährlichen Channel.</span><span class="sxs-lookup"><span data-stu-id="1fcc0-121">Semi-annual Channel.</span></span> <span data-ttu-id="1fcc0-122">Gerät ruft Feature Updates aus Semikolons jährlichen Channel ab.</span><span class="sxs-lookup"><span data-stu-id="1fcc0-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="1fcc0-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="1fcc0-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="1fcc0-124">3</span><span class="sxs-lookup"><span data-stu-id="1fcc0-124">3</span></span>|<span data-ttu-id="1fcc0-125">Erstellen von Windows-Insider - Fast</span><span class="sxs-lookup"><span data-stu-id="1fcc0-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="1fcc0-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="1fcc0-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="1fcc0-127">4</span><span class="sxs-lookup"><span data-stu-id="1fcc0-127">4</span></span>|<span data-ttu-id="1fcc0-128">Erstellen von Windows-Insider - langsam</span><span class="sxs-lookup"><span data-stu-id="1fcc0-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="1fcc0-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="1fcc0-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="1fcc0-130">5</span><span class="sxs-lookup"><span data-stu-id="1fcc0-130">5</span></span>|<span data-ttu-id="1fcc0-131">Windows-Insider Build-Version</span><span class="sxs-lookup"><span data-stu-id="1fcc0-131">Release Windows Insider build</span></span>|




