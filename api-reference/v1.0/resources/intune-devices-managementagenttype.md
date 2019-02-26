---
title: managementAgentType-Enumerationstyp
description: Verwaltungs-Agenttyp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9743c9c83e34a0c58dee78e73839f8fdcaaf2cda
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251566"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="819da-103">managementAgentType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="819da-103">managementAgentType enum type</span></span>

> <span data-ttu-id="819da-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="819da-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="819da-105">Verwaltungs-Agenttyp.</span><span class="sxs-lookup"><span data-stu-id="819da-105">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="819da-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="819da-106">Members</span></span>
|<span data-ttu-id="819da-107">Element</span><span class="sxs-lookup"><span data-stu-id="819da-107">Member</span></span>|<span data-ttu-id="819da-108">Wert</span><span class="sxs-lookup"><span data-stu-id="819da-108">Value</span></span>|<span data-ttu-id="819da-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="819da-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="819da-110">EAS</span><span class="sxs-lookup"><span data-stu-id="819da-110">eas</span></span>|<span data-ttu-id="819da-111">1</span><span class="sxs-lookup"><span data-stu-id="819da-111">1</span></span>|<span data-ttu-id="819da-112">Das Gerät wird von Exchange Server verwaltet.</span><span class="sxs-lookup"><span data-stu-id="819da-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="819da-113">MDM</span><span class="sxs-lookup"><span data-stu-id="819da-113">mdm</span></span>|<span data-ttu-id="819da-114">2</span><span class="sxs-lookup"><span data-stu-id="819da-114">2</span></span>|<span data-ttu-id="819da-115">Das Gerät wird von InTune MDM verwaltet.</span><span class="sxs-lookup"><span data-stu-id="819da-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="819da-116">easMdm</span><span class="sxs-lookup"><span data-stu-id="819da-116">easMdm</span></span>|<span data-ttu-id="819da-117">3</span><span class="sxs-lookup"><span data-stu-id="819da-117">3</span></span>|<span data-ttu-id="819da-118">Das Gerät wird sowohl von Exchange Server als auch von InTune MDM verwaltet.</span><span class="sxs-lookup"><span data-stu-id="819da-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="819da-119">intuneClient</span><span class="sxs-lookup"><span data-stu-id="819da-119">intuneClient</span></span>|<span data-ttu-id="819da-120">4</span><span class="sxs-lookup"><span data-stu-id="819da-120">4</span></span>|<span data-ttu-id="819da-121">InTune-Client verwaltet.</span><span class="sxs-lookup"><span data-stu-id="819da-121">Intune client managed.</span></span>|
|<span data-ttu-id="819da-122">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="819da-122">easIntuneClient</span></span>|<span data-ttu-id="819da-123">5</span><span class="sxs-lookup"><span data-stu-id="819da-123">5</span></span>|<span data-ttu-id="819da-124">Das Gerät ist EAS und InTune-Client Dual verwaltet.</span><span class="sxs-lookup"><span data-stu-id="819da-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="819da-125">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="819da-125">configurationManagerClient</span></span>|<span data-ttu-id="819da-126">8</span><span class="sxs-lookup"><span data-stu-id="819da-126">8</span></span>|<span data-ttu-id="819da-127">Das Gerät wird von Configuration Manager verwaltet.</span><span class="sxs-lookup"><span data-stu-id="819da-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="819da-128">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="819da-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="819da-129">10</span><span class="sxs-lookup"><span data-stu-id="819da-129">10</span></span>|<span data-ttu-id="819da-130">Das Gerät wird von Configuration Manager und MDM verwaltet.</span><span class="sxs-lookup"><span data-stu-id="819da-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="819da-131">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="819da-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="819da-132">11</span><span class="sxs-lookup"><span data-stu-id="819da-132">11</span></span>|<span data-ttu-id="819da-133">Das Gerät wird von Configuration Manager, MDM und EAS verwaltet.</span><span class="sxs-lookup"><span data-stu-id="819da-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="819da-134">unknown</span><span class="sxs-lookup"><span data-stu-id="819da-134">unknown</span></span>|<span data-ttu-id="819da-135">16</span><span class="sxs-lookup"><span data-stu-id="819da-135">16</span></span>|<span data-ttu-id="819da-136">UnBekannter Verwaltungs-Agenttyp.</span><span class="sxs-lookup"><span data-stu-id="819da-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="819da-137">JAMF</span><span class="sxs-lookup"><span data-stu-id="819da-137">jamf</span></span>|<span data-ttu-id="819da-138">32</span><span class="sxs-lookup"><span data-stu-id="819da-138">32</span></span>|<span data-ttu-id="819da-139">Die Geräteattribute werden aus JAMF abgerufen.</span><span class="sxs-lookup"><span data-stu-id="819da-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="819da-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="819da-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="819da-141">64</span><span class="sxs-lookup"><span data-stu-id="819da-141">64</span></span>|<span data-ttu-id="819da-142">Das Gerät wird von Googles CloudDPC verwaltet.</span><span class="sxs-lookup"><span data-stu-id="819da-142">The device is managed by Google's CloudDPC.</span></span>|



