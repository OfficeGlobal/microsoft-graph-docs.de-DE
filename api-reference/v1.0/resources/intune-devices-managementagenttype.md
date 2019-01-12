---
title: ManagementAgentType Enum-Typ
description: Typ der Management Agent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b76231a2781a153c5384c1dc3efdf8facec04dcc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966167"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="ae65c-103">ManagementAgentType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="ae65c-103">managementAgentType enum type</span></span>

> <span data-ttu-id="ae65c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ae65c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae65c-105">Typ der Management Agent.</span><span class="sxs-lookup"><span data-stu-id="ae65c-105">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="ae65c-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="ae65c-106">Members</span></span>
|<span data-ttu-id="ae65c-107">Element</span><span class="sxs-lookup"><span data-stu-id="ae65c-107">Member</span></span>|<span data-ttu-id="ae65c-108">Wert</span><span class="sxs-lookup"><span data-stu-id="ae65c-108">Value</span></span>|<span data-ttu-id="ae65c-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae65c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae65c-110">EAS</span><span class="sxs-lookup"><span data-stu-id="ae65c-110">eas</span></span>|<span data-ttu-id="ae65c-111">1</span><span class="sxs-lookup"><span data-stu-id="ae65c-111">1</span></span>|<span data-ttu-id="ae65c-112">Das Gerät wird vom Exchange-Server verwaltet.</span><span class="sxs-lookup"><span data-stu-id="ae65c-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="ae65c-113">MDM</span><span class="sxs-lookup"><span data-stu-id="ae65c-113">mdm</span></span>|<span data-ttu-id="ae65c-114">2</span><span class="sxs-lookup"><span data-stu-id="ae65c-114">2</span></span>|<span data-ttu-id="ae65c-115">Das Gerät wird durch Intune MDM verwaltet.</span><span class="sxs-lookup"><span data-stu-id="ae65c-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="ae65c-116">easMdm</span><span class="sxs-lookup"><span data-stu-id="ae65c-116">easMdm</span></span>|<span data-ttu-id="ae65c-117">3</span><span class="sxs-lookup"><span data-stu-id="ae65c-117">3</span></span>|<span data-ttu-id="ae65c-118">Das Gerät wird von Exchange Server und Intune MDM verwaltet.</span><span class="sxs-lookup"><span data-stu-id="ae65c-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="ae65c-119">intuneClient</span><span class="sxs-lookup"><span data-stu-id="ae65c-119">intuneClient</span></span>|<span data-ttu-id="ae65c-120">4</span><span class="sxs-lookup"><span data-stu-id="ae65c-120">4</span></span>|<span data-ttu-id="ae65c-121">Intune Client verwaltet.</span><span class="sxs-lookup"><span data-stu-id="ae65c-121">Intune client managed.</span></span>|
|<span data-ttu-id="ae65c-122">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="ae65c-122">easIntuneClient</span></span>|<span data-ttu-id="ae65c-123">5</span><span class="sxs-lookup"><span data-stu-id="ae65c-123">5</span></span>|<span data-ttu-id="ae65c-124">Das Gerät ist EAS Intune-Client und zwei verwaltet.</span><span class="sxs-lookup"><span data-stu-id="ae65c-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="ae65c-125">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="ae65c-125">configurationManagerClient</span></span>|<span data-ttu-id="ae65c-126">8</span><span class="sxs-lookup"><span data-stu-id="ae65c-126">8</span></span>|<span data-ttu-id="ae65c-127">Das Gerät wird vom Konfigurations-Manager verwaltet.</span><span class="sxs-lookup"><span data-stu-id="ae65c-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="ae65c-128">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="ae65c-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="ae65c-129">10</span><span class="sxs-lookup"><span data-stu-id="ae65c-129">10</span></span>|<span data-ttu-id="ae65c-130">Das Gerät wird vom Konfigurations-Manager und MDM verwaltet.</span><span class="sxs-lookup"><span data-stu-id="ae65c-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="ae65c-131">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="ae65c-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="ae65c-132">11</span><span class="sxs-lookup"><span data-stu-id="ae65c-132">11</span></span>|<span data-ttu-id="ae65c-133">Das Gerät wird vom Konfigurations-Manager, MDM und Eas verwaltet.</span><span class="sxs-lookup"><span data-stu-id="ae65c-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="ae65c-134">unknown</span><span class="sxs-lookup"><span data-stu-id="ae65c-134">unknown</span></span>|<span data-ttu-id="ae65c-135">16</span><span class="sxs-lookup"><span data-stu-id="ae65c-135">16</span></span>|<span data-ttu-id="ae65c-136">Unbekannte Management Agent-Typ.</span><span class="sxs-lookup"><span data-stu-id="ae65c-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="ae65c-137">jamf</span><span class="sxs-lookup"><span data-stu-id="ae65c-137">jamf</span></span>|<span data-ttu-id="ae65c-138">32</span><span class="sxs-lookup"><span data-stu-id="ae65c-138">32</span></span>|<span data-ttu-id="ae65c-139">Das Gerätattribute werden aus Jamf abgerufen.</span><span class="sxs-lookup"><span data-stu-id="ae65c-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="ae65c-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="ae65c-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="ae65c-141">64</span><span class="sxs-lookup"><span data-stu-id="ae65c-141">64</span></span>|<span data-ttu-id="ae65c-142">Das Gerät wird von Google CloudDPC verwaltet.</span><span class="sxs-lookup"><span data-stu-id="ae65c-142">The device is managed by Google's CloudDPC.</span></span>|



