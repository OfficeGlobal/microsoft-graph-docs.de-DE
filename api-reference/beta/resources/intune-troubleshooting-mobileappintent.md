---
title: mobileAppIntent-Enumerationstyp
description: Gibt den Status der mobilen App auf dem Gerät an.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1df0b41636668e0ebcc38dfb6b399a73551658d1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171043"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="1a1c5-103">mobileAppIntent-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="1a1c5-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="1a1c5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1a1c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a1c5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1a1c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a1c5-106">Gibt den Status der mobilen App auf dem Gerät an.</span><span class="sxs-lookup"><span data-stu-id="1a1c5-106">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="1a1c5-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="1a1c5-107">Members</span></span>
|<span data-ttu-id="1a1c5-108">Element</span><span class="sxs-lookup"><span data-stu-id="1a1c5-108">Member</span></span>|<span data-ttu-id="1a1c5-109">Wert</span><span class="sxs-lookup"><span data-stu-id="1a1c5-109">Value</span></span>|<span data-ttu-id="1a1c5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a1c5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a1c5-111">Verfügbar</span><span class="sxs-lookup"><span data-stu-id="1a1c5-111">available</span></span>|<span data-ttu-id="1a1c5-112">0</span><span class="sxs-lookup"><span data-stu-id="1a1c5-112">0</span></span>|<span data-ttu-id="1a1c5-113">Available</span><span class="sxs-lookup"><span data-stu-id="1a1c5-113">Available</span></span>|
|<span data-ttu-id="1a1c5-114">Nichtin</span><span class="sxs-lookup"><span data-stu-id="1a1c5-114">notAvailable</span></span>|<span data-ttu-id="1a1c5-115">1</span><span class="sxs-lookup"><span data-stu-id="1a1c5-115">1</span></span>|<span data-ttu-id="1a1c5-116">Nicht verfügbar</span><span class="sxs-lookup"><span data-stu-id="1a1c5-116">Not Available</span></span>|
|<span data-ttu-id="1a1c5-117">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="1a1c5-117">requiredInstall</span></span>|<span data-ttu-id="1a1c5-118">2</span><span class="sxs-lookup"><span data-stu-id="1a1c5-118">2</span></span>|<span data-ttu-id="1a1c5-119">Erforderliche Installation</span><span class="sxs-lookup"><span data-stu-id="1a1c5-119">Required Install</span></span>|
|<span data-ttu-id="1a1c5-120">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="1a1c5-120">requiredUninstall</span></span>|<span data-ttu-id="1a1c5-121">3</span><span class="sxs-lookup"><span data-stu-id="1a1c5-121">3</span></span>|<span data-ttu-id="1a1c5-122">Erforderliche deInstallation</span><span class="sxs-lookup"><span data-stu-id="1a1c5-122">Required Uninstall</span></span>|
|<span data-ttu-id="1a1c5-123">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="1a1c5-123">requiredAndAvailableInstall</span></span>|<span data-ttu-id="1a1c5-124">4</span><span class="sxs-lookup"><span data-stu-id="1a1c5-124">4</span></span>|<span data-ttu-id="1a1c5-125">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="1a1c5-125">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="1a1c5-126">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="1a1c5-126">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="1a1c5-127">5</span><span class="sxs-lookup"><span data-stu-id="1a1c5-127">5</span></span>|<span data-ttu-id="1a1c5-128">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="1a1c5-128">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="1a1c5-129">ausschließen</span><span class="sxs-lookup"><span data-stu-id="1a1c5-129">exclude</span></span>|<span data-ttu-id="1a1c5-130">6</span><span class="sxs-lookup"><span data-stu-id="1a1c5-130">6</span></span>|<span data-ttu-id="1a1c5-131">Ausschließen</span><span class="sxs-lookup"><span data-stu-id="1a1c5-131">Exclude</span></span>|




