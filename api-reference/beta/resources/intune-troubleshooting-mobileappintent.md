---
title: MobileAppIntent Enum-Typ
description: Gibt den Status der mobilen app auf dem Gerät.
author: tfitzmac
ms.openlocfilehash: 0a230279a947ab60314a53872670fff871eff745
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347229"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="64bd4-103">MobileAppIntent Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="64bd4-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="64bd4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="64bd4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64bd4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="64bd4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64bd4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="64bd4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64bd4-107">Gibt den Status der mobilen app auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="64bd4-107">Indicates the status of the mobile app on the device.</span></span>
## <a name="members"></a><span data-ttu-id="64bd4-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="64bd4-108">Members</span></span>
|<span data-ttu-id="64bd4-109">Member</span><span class="sxs-lookup"><span data-stu-id="64bd4-109">Member</span></span>|<span data-ttu-id="64bd4-110">Wert</span><span class="sxs-lookup"><span data-stu-id="64bd4-110">Value</span></span>|<span data-ttu-id="64bd4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="64bd4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64bd4-112">Verfügbar</span><span class="sxs-lookup"><span data-stu-id="64bd4-112">available</span></span>|<span data-ttu-id="64bd4-113">0</span><span class="sxs-lookup"><span data-stu-id="64bd4-113">0</span></span>|<span data-ttu-id="64bd4-114">Available</span><span class="sxs-lookup"><span data-stu-id="64bd4-114">Available</span></span>|
|<span data-ttu-id="64bd4-115">nicht verfügbar</span><span class="sxs-lookup"><span data-stu-id="64bd4-115">notAvailable</span></span>|<span data-ttu-id="64bd4-116">1</span><span class="sxs-lookup"><span data-stu-id="64bd4-116">1</span></span>|<span data-ttu-id="64bd4-117">Nicht verfügbar</span><span class="sxs-lookup"><span data-stu-id="64bd4-117">Not Available</span></span>|
|<span data-ttu-id="64bd4-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="64bd4-118">requiredInstall</span></span>|<span data-ttu-id="64bd4-119">2</span><span class="sxs-lookup"><span data-stu-id="64bd4-119">2</span></span>|<span data-ttu-id="64bd4-120">Installation erforderlich</span><span class="sxs-lookup"><span data-stu-id="64bd4-120">Required Install</span></span>|
|<span data-ttu-id="64bd4-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="64bd4-121">requiredUninstall</span></span>|<span data-ttu-id="64bd4-122">3</span><span class="sxs-lookup"><span data-stu-id="64bd4-122">3</span></span>|<span data-ttu-id="64bd4-123">Erforderliche Deinstallation</span><span class="sxs-lookup"><span data-stu-id="64bd4-123">Required Uninstall</span></span>|
|<span data-ttu-id="64bd4-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="64bd4-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="64bd4-125">4</span><span class="sxs-lookup"><span data-stu-id="64bd4-125">4</span></span>|<span data-ttu-id="64bd4-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="64bd4-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="64bd4-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="64bd4-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="64bd4-128">5</span><span class="sxs-lookup"><span data-stu-id="64bd4-128">5</span></span>|<span data-ttu-id="64bd4-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="64bd4-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="64bd4-130">Ausschließen</span><span class="sxs-lookup"><span data-stu-id="64bd4-130">exclude</span></span>|<span data-ttu-id="64bd4-131">6</span><span class="sxs-lookup"><span data-stu-id="64bd4-131">6</span></span>|<span data-ttu-id="64bd4-132">Ausschließen</span><span class="sxs-lookup"><span data-stu-id="64bd4-132">Exclude</span></span>|





