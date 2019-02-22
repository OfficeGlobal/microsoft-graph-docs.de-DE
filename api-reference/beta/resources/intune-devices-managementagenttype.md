---
title: managementAgentType-Enumerationstyp
description: Verwaltungs-Agenttyp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb948626035bed2dac7ee18d103aa083bd0f2aeb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172541"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="228e9-103">managementAgentType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="228e9-103">managementAgentType enum type</span></span>

> <span data-ttu-id="228e9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="228e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="228e9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="228e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="228e9-106">Verwaltungs-Agenttyp.</span><span class="sxs-lookup"><span data-stu-id="228e9-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="228e9-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="228e9-107">Members</span></span>
|<span data-ttu-id="228e9-108">Element</span><span class="sxs-lookup"><span data-stu-id="228e9-108">Member</span></span>|<span data-ttu-id="228e9-109">Wert</span><span class="sxs-lookup"><span data-stu-id="228e9-109">Value</span></span>|<span data-ttu-id="228e9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="228e9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="228e9-111">EAS</span><span class="sxs-lookup"><span data-stu-id="228e9-111">eas</span></span>|<span data-ttu-id="228e9-112">1</span><span class="sxs-lookup"><span data-stu-id="228e9-112">1</span></span>|<span data-ttu-id="228e9-113">Das Gerät wird von Exchange Server verwaltet.</span><span class="sxs-lookup"><span data-stu-id="228e9-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="228e9-114">MDM</span><span class="sxs-lookup"><span data-stu-id="228e9-114">mdm</span></span>|<span data-ttu-id="228e9-115">2</span><span class="sxs-lookup"><span data-stu-id="228e9-115">2</span></span>|<span data-ttu-id="228e9-116">Das Gerät wird von InTune MDM verwaltet.</span><span class="sxs-lookup"><span data-stu-id="228e9-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="228e9-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="228e9-117">easMdm</span></span>|<span data-ttu-id="228e9-118">3</span><span class="sxs-lookup"><span data-stu-id="228e9-118">3</span></span>|<span data-ttu-id="228e9-119">Das Gerät wird sowohl von Exchange Server als auch von InTune MDM verwaltet.</span><span class="sxs-lookup"><span data-stu-id="228e9-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="228e9-120">intuneClient</span><span class="sxs-lookup"><span data-stu-id="228e9-120">intuneClient</span></span>|<span data-ttu-id="228e9-121">4</span><span class="sxs-lookup"><span data-stu-id="228e9-121">4</span></span>|<span data-ttu-id="228e9-122">InTune-Client verwaltet.</span><span class="sxs-lookup"><span data-stu-id="228e9-122">Intune client managed.</span></span>|
|<span data-ttu-id="228e9-123">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="228e9-123">easIntuneClient</span></span>|<span data-ttu-id="228e9-124">5</span><span class="sxs-lookup"><span data-stu-id="228e9-124">5</span></span>|<span data-ttu-id="228e9-125">Das Gerät ist EAS und InTune-Client Dual verwaltet.</span><span class="sxs-lookup"><span data-stu-id="228e9-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="228e9-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="228e9-126">configurationManagerClient</span></span>|<span data-ttu-id="228e9-127">8</span><span class="sxs-lookup"><span data-stu-id="228e9-127">8</span></span>|<span data-ttu-id="228e9-128">Das Gerät wird von Configuration Manager verwaltet.</span><span class="sxs-lookup"><span data-stu-id="228e9-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="228e9-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="228e9-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="228e9-130">10</span><span class="sxs-lookup"><span data-stu-id="228e9-130">10</span></span>|<span data-ttu-id="228e9-131">Das Gerät wird von Configuration Manager und MDM verwaltet.</span><span class="sxs-lookup"><span data-stu-id="228e9-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="228e9-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="228e9-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="228e9-133">11</span><span class="sxs-lookup"><span data-stu-id="228e9-133">11</span></span>|<span data-ttu-id="228e9-134">Das Gerät wird von Configuration Manager, MDM und EAS verwaltet.</span><span class="sxs-lookup"><span data-stu-id="228e9-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="228e9-135">unknown</span><span class="sxs-lookup"><span data-stu-id="228e9-135">unknown</span></span>|<span data-ttu-id="228e9-136">16</span><span class="sxs-lookup"><span data-stu-id="228e9-136">16</span></span>|<span data-ttu-id="228e9-137">UnBekannter Verwaltungs-Agenttyp.</span><span class="sxs-lookup"><span data-stu-id="228e9-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="228e9-138">JAMF</span><span class="sxs-lookup"><span data-stu-id="228e9-138">jamf</span></span>|<span data-ttu-id="228e9-139">32</span><span class="sxs-lookup"><span data-stu-id="228e9-139">32</span></span>|<span data-ttu-id="228e9-140">Die Geräteattribute werden aus JAMF abgerufen.</span><span class="sxs-lookup"><span data-stu-id="228e9-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="228e9-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="228e9-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="228e9-142">64</span><span class="sxs-lookup"><span data-stu-id="228e9-142">64</span></span>|<span data-ttu-id="228e9-143">Das Gerät wird von Googles CloudDPC verwaltet.</span><span class="sxs-lookup"><span data-stu-id="228e9-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="228e9-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="228e9-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="228e9-145">258</span><span class="sxs-lookup"><span data-stu-id="228e9-145">258</span></span>|<span data-ttu-id="228e9-146">Dieses Gerät wird von Microsoft 365 über InTune verwaltet.</span><span class="sxs-lookup"><span data-stu-id="228e9-146">This device is managed by Microsoft 365 through Intune.</span></span>|




