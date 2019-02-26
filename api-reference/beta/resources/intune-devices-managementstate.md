---
title: managementState-Enumerationstyp
description: Verwaltungsstatus des Geräts in Microsoft InTune
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a53b07f89ee551d3e559a42bbe23c5fba808f20
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174144"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="bbc86-103">managementState-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="bbc86-103">managementState enum type</span></span>

> <span data-ttu-id="bbc86-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bbc86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbc86-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bbc86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbc86-106">Verwaltungsstatus des Geräts in Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="bbc86-106">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="bbc86-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="bbc86-107">Members</span></span>
|<span data-ttu-id="bbc86-108">Element</span><span class="sxs-lookup"><span data-stu-id="bbc86-108">Member</span></span>|<span data-ttu-id="bbc86-109">Wert</span><span class="sxs-lookup"><span data-stu-id="bbc86-109">Value</span></span>|<span data-ttu-id="bbc86-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bbc86-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbc86-111">verwaltete</span><span class="sxs-lookup"><span data-stu-id="bbc86-111">managed</span></span>|<span data-ttu-id="bbc86-112">0</span><span class="sxs-lookup"><span data-stu-id="bbc86-112">0</span></span>|<span data-ttu-id="bbc86-113">Das Gerät ist unter Verwaltung</span><span class="sxs-lookup"><span data-stu-id="bbc86-113">The device is under management</span></span>|
|<span data-ttu-id="bbc86-114">retirePending</span><span class="sxs-lookup"><span data-stu-id="bbc86-114">retirePending</span></span>|<span data-ttu-id="bbc86-115">1</span><span class="sxs-lookup"><span data-stu-id="bbc86-115">1</span></span>|<span data-ttu-id="bbc86-116">Ein Ruhestands Befehl tritt auf dem Gerät auf und wird während der Registrierung von der Verwaltung abgemeldet.</span><span class="sxs-lookup"><span data-stu-id="bbc86-116">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="bbc86-117">retireFailed</span><span class="sxs-lookup"><span data-stu-id="bbc86-117">retireFailed</span></span>|<span data-ttu-id="bbc86-118">2</span><span class="sxs-lookup"><span data-stu-id="bbc86-118">2</span></span>|<span data-ttu-id="bbc86-119">Fehler beim Ausführen des Befehls auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="bbc86-119">Retire command failed on the device</span></span>|
|<span data-ttu-id="bbc86-120">wipePending</span><span class="sxs-lookup"><span data-stu-id="bbc86-120">wipePending</span></span>|<span data-ttu-id="bbc86-121">3</span><span class="sxs-lookup"><span data-stu-id="bbc86-121">3</span></span>|<span data-ttu-id="bbc86-122">Ein Löschbefehl ist auf dem Gerät und während der Registrierung von der Verwaltung</span><span class="sxs-lookup"><span data-stu-id="bbc86-122">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="bbc86-123">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="bbc86-123">wipeFailed</span></span>|<span data-ttu-id="bbc86-124">4</span><span class="sxs-lookup"><span data-stu-id="bbc86-124">4</span></span>|<span data-ttu-id="bbc86-125">Löschbefehl auf dem Gerät fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="bbc86-125">Wipe command failed on the device</span></span>|
|<span data-ttu-id="bbc86-126">fehlerhaft</span><span class="sxs-lookup"><span data-stu-id="bbc86-126">unhealthy</span></span>|<span data-ttu-id="bbc86-127">5</span><span class="sxs-lookup"><span data-stu-id="bbc86-127">5</span></span>|<span data-ttu-id="bbc86-128">Das Gerät ist fehlerhaft.</span><span class="sxs-lookup"><span data-stu-id="bbc86-128">The device is unhealthy.</span></span>|
|<span data-ttu-id="bbc86-129">deletePending</span><span class="sxs-lookup"><span data-stu-id="bbc86-129">deletePending</span></span>|<span data-ttu-id="bbc86-130">6</span><span class="sxs-lookup"><span data-stu-id="bbc86-130">6</span></span>|<span data-ttu-id="bbc86-131">Auf dem Gerät tritt ein Löschbefehl auf.</span><span class="sxs-lookup"><span data-stu-id="bbc86-131">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="bbc86-132">retireIssued</span><span class="sxs-lookup"><span data-stu-id="bbc86-132">retireIssued</span></span>|<span data-ttu-id="bbc86-133">7</span><span class="sxs-lookup"><span data-stu-id="bbc86-133">7</span></span>|<span data-ttu-id="bbc86-134">Für das Gerät wurde ein Ruhestands Befehl ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="bbc86-134">A retire command was issued for the device</span></span>|
|<span data-ttu-id="bbc86-135">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="bbc86-135">wipeIssued</span></span>|<span data-ttu-id="bbc86-136">8</span><span class="sxs-lookup"><span data-stu-id="bbc86-136">8</span></span>|<span data-ttu-id="bbc86-137">Für das Gerät wurde ein Löschbefehl ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="bbc86-137">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="bbc86-138">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="bbc86-138">wipeCanceled</span></span>|<span data-ttu-id="bbc86-139">9</span><span class="sxs-lookup"><span data-stu-id="bbc86-139">9</span></span>|<span data-ttu-id="bbc86-140">Ein Löschbefehl für dieses Gerät wurde abgebrochen</span><span class="sxs-lookup"><span data-stu-id="bbc86-140">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="bbc86-141">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="bbc86-141">retireCanceled</span></span>|<span data-ttu-id="bbc86-142">10</span><span class="sxs-lookup"><span data-stu-id="bbc86-142">10</span></span>|<span data-ttu-id="bbc86-143">Ein Ruhestands Befehl für dieses Gerät wurde abgebrochen</span><span class="sxs-lookup"><span data-stu-id="bbc86-143">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="bbc86-144">ermittelt</span><span class="sxs-lookup"><span data-stu-id="bbc86-144">discovered</span></span>|<span data-ttu-id="bbc86-145">11</span><span class="sxs-lookup"><span data-stu-id="bbc86-145">11</span></span>|<span data-ttu-id="bbc86-146">Das Gerät wurde ermittelt, aber nicht vollständig registriert.</span><span class="sxs-lookup"><span data-stu-id="bbc86-146">The device is discovered but not fully enrolled.</span></span>|




