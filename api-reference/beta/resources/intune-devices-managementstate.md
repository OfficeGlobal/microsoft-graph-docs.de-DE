---
title: ManagementState Enum-Typ
description: Verwaltungsstatus des Geräts in Microsoft Intune.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8d0801949125f3b0cceb865ac1f8546195112e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420017"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="327a5-103">ManagementState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="327a5-103">managementState enum type</span></span>

> <span data-ttu-id="327a5-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="327a5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="327a5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="327a5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="327a5-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="327a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="327a5-107">Verwaltungsstatus des Geräts in Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="327a5-107">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="327a5-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="327a5-108">Members</span></span>
|<span data-ttu-id="327a5-109">Member</span><span class="sxs-lookup"><span data-stu-id="327a5-109">Member</span></span>|<span data-ttu-id="327a5-110">Wert</span><span class="sxs-lookup"><span data-stu-id="327a5-110">Value</span></span>|<span data-ttu-id="327a5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="327a5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="327a5-112">verwaltete</span><span class="sxs-lookup"><span data-stu-id="327a5-112">managed</span></span>|<span data-ttu-id="327a5-113">0</span><span class="sxs-lookup"><span data-stu-id="327a5-113">0</span></span>|<span data-ttu-id="327a5-114">Das Gerät ist, klicken Sie unter Verwaltung</span><span class="sxs-lookup"><span data-stu-id="327a5-114">The device is under management</span></span>|
|<span data-ttu-id="327a5-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="327a5-115">retirePending</span></span>|<span data-ttu-id="327a5-116">1</span><span class="sxs-lookup"><span data-stu-id="327a5-116">1</span></span>|<span data-ttu-id="327a5-117">Ein Außerkraftsetzungsrichtlinie Befehl ist nicht mehr auftritt, auf dem Gerät und gerade unenrolling aus der Verwaltung</span><span class="sxs-lookup"><span data-stu-id="327a5-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="327a5-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="327a5-118">retireFailed</span></span>|<span data-ttu-id="327a5-119">2</span><span class="sxs-lookup"><span data-stu-id="327a5-119">2</span></span>|<span data-ttu-id="327a5-120">Stilllegung der Befehl auf dem Gerät fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="327a5-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="327a5-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="327a5-121">wipePending</span></span>|<span data-ttu-id="327a5-122">3</span><span class="sxs-lookup"><span data-stu-id="327a5-122">3</span></span>|<span data-ttu-id="327a5-123">Ein Remotegerätzurücksetzung Befehl ist nicht mehr auftritt, auf dem Gerät und gerade unenrolling aus der Verwaltung</span><span class="sxs-lookup"><span data-stu-id="327a5-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="327a5-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="327a5-124">wipeFailed</span></span>|<span data-ttu-id="327a5-125">4</span><span class="sxs-lookup"><span data-stu-id="327a5-125">4</span></span>|<span data-ttu-id="327a5-126">Wischen Sie Fehler auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="327a5-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="327a5-127">fehlerhaft</span><span class="sxs-lookup"><span data-stu-id="327a5-127">unhealthy</span></span>|<span data-ttu-id="327a5-128">5</span><span class="sxs-lookup"><span data-stu-id="327a5-128">5</span></span>|<span data-ttu-id="327a5-129">Das Gerät ist fehlerhaft.</span><span class="sxs-lookup"><span data-stu-id="327a5-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="327a5-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="327a5-130">deletePending</span></span>|<span data-ttu-id="327a5-131">6</span><span class="sxs-lookup"><span data-stu-id="327a5-131">6</span></span>|<span data-ttu-id="327a5-132">Ein Löschbefehl ist nicht mehr auftritt, auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="327a5-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="327a5-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="327a5-133">retireIssued</span></span>|<span data-ttu-id="327a5-134">7</span><span class="sxs-lookup"><span data-stu-id="327a5-134">7</span></span>|<span data-ttu-id="327a5-135">Ein Befehl Außerkraftsetzungsrichtlinie wurde für das Gerät ausgestellt.</span><span class="sxs-lookup"><span data-stu-id="327a5-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="327a5-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="327a5-136">wipeIssued</span></span>|<span data-ttu-id="327a5-137">8</span><span class="sxs-lookup"><span data-stu-id="327a5-137">8</span></span>|<span data-ttu-id="327a5-138">Ein Befehl Remotegerätzurücksetzung wurde für das Gerät ausgestellt.</span><span class="sxs-lookup"><span data-stu-id="327a5-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="327a5-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="327a5-139">wipeCanceled</span></span>|<span data-ttu-id="327a5-140">9</span><span class="sxs-lookup"><span data-stu-id="327a5-140">9</span></span>|<span data-ttu-id="327a5-141">Ein Befehl Remotegerätzurücksetzung für dieses Gerät wurde abgebrochen</span><span class="sxs-lookup"><span data-stu-id="327a5-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="327a5-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="327a5-142">retireCanceled</span></span>|<span data-ttu-id="327a5-143">10</span><span class="sxs-lookup"><span data-stu-id="327a5-143">10</span></span>|<span data-ttu-id="327a5-144">Ein Befehl Außerkraftsetzungsrichtlinie für dieses Gerät wurde abgebrochen</span><span class="sxs-lookup"><span data-stu-id="327a5-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="327a5-145">ermittelt</span><span class="sxs-lookup"><span data-stu-id="327a5-145">discovered</span></span>|<span data-ttu-id="327a5-146">11</span><span class="sxs-lookup"><span data-stu-id="327a5-146">11</span></span>|<span data-ttu-id="327a5-147">Das Gerät wird erkannt, aber nicht vollständig registriert.</span><span class="sxs-lookup"><span data-stu-id="327a5-147">The device is discovered but not fully enrolled.</span></span>|




