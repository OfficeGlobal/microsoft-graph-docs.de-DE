---
title: MobileAppIntent Enum-Typ
description: Gibt den Status der mobilen app auf dem Gerät.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7cd26912406fc428f28c65abce2169c14d686342
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933379"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="0bb64-103">MobileAppIntent Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="0bb64-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="0bb64-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0bb64-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0bb64-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0bb64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0bb64-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0bb64-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bb64-107">Gibt den Status der mobilen app auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="0bb64-107">Indicates the status of the mobile app on the device.</span></span>
## <a name="members"></a><span data-ttu-id="0bb64-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="0bb64-108">Members</span></span>
|<span data-ttu-id="0bb64-109">Element</span><span class="sxs-lookup"><span data-stu-id="0bb64-109">Member</span></span>|<span data-ttu-id="0bb64-110">Wert</span><span class="sxs-lookup"><span data-stu-id="0bb64-110">Value</span></span>|<span data-ttu-id="0bb64-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0bb64-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bb64-112">Verfügbar</span><span class="sxs-lookup"><span data-stu-id="0bb64-112">available</span></span>|<span data-ttu-id="0bb64-113">0</span><span class="sxs-lookup"><span data-stu-id="0bb64-113">0</span></span>|<span data-ttu-id="0bb64-114">Available</span><span class="sxs-lookup"><span data-stu-id="0bb64-114">Available</span></span>|
|<span data-ttu-id="0bb64-115">nicht verfügbar</span><span class="sxs-lookup"><span data-stu-id="0bb64-115">notAvailable</span></span>|<span data-ttu-id="0bb64-116">1</span><span class="sxs-lookup"><span data-stu-id="0bb64-116">1</span></span>|<span data-ttu-id="0bb64-117">Nicht verfügbar</span><span class="sxs-lookup"><span data-stu-id="0bb64-117">Not Available</span></span>|
|<span data-ttu-id="0bb64-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="0bb64-118">requiredInstall</span></span>|<span data-ttu-id="0bb64-119">2</span><span class="sxs-lookup"><span data-stu-id="0bb64-119">2</span></span>|<span data-ttu-id="0bb64-120">Installation erforderlich</span><span class="sxs-lookup"><span data-stu-id="0bb64-120">Required Install</span></span>|
|<span data-ttu-id="0bb64-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="0bb64-121">requiredUninstall</span></span>|<span data-ttu-id="0bb64-122">3</span><span class="sxs-lookup"><span data-stu-id="0bb64-122">3</span></span>|<span data-ttu-id="0bb64-123">Erforderliche Deinstallation</span><span class="sxs-lookup"><span data-stu-id="0bb64-123">Required Uninstall</span></span>|
|<span data-ttu-id="0bb64-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="0bb64-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="0bb64-125">4</span><span class="sxs-lookup"><span data-stu-id="0bb64-125">4</span></span>|<span data-ttu-id="0bb64-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="0bb64-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="0bb64-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="0bb64-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="0bb64-128">5</span><span class="sxs-lookup"><span data-stu-id="0bb64-128">5</span></span>|<span data-ttu-id="0bb64-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="0bb64-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="0bb64-130">Ausschließen</span><span class="sxs-lookup"><span data-stu-id="0bb64-130">exclude</span></span>|<span data-ttu-id="0bb64-131">6</span><span class="sxs-lookup"><span data-stu-id="0bb64-131">6</span></span>|<span data-ttu-id="0bb64-132">Ausschließen</span><span class="sxs-lookup"><span data-stu-id="0bb64-132">Exclude</span></span>|





