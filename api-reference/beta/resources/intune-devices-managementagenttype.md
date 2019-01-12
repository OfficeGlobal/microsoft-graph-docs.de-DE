---
title: ManagementAgentType Enum-Typ
description: Typ der Management Agent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1711ad647afabc2b8877bd2f99b049bd1c1dd4e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914283"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="b90b3-103">ManagementAgentType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="b90b3-103">managementAgentType enum type</span></span>

> <span data-ttu-id="b90b3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b90b3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b90b3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b90b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b90b3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b90b3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b90b3-107">Typ der Management Agent.</span><span class="sxs-lookup"><span data-stu-id="b90b3-107">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="b90b3-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="b90b3-108">Members</span></span>
|<span data-ttu-id="b90b3-109">Element</span><span class="sxs-lookup"><span data-stu-id="b90b3-109">Member</span></span>|<span data-ttu-id="b90b3-110">Wert</span><span class="sxs-lookup"><span data-stu-id="b90b3-110">Value</span></span>|<span data-ttu-id="b90b3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b90b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b90b3-112">EAS</span><span class="sxs-lookup"><span data-stu-id="b90b3-112">eas</span></span>|<span data-ttu-id="b90b3-113">1</span><span class="sxs-lookup"><span data-stu-id="b90b3-113">1</span></span>|<span data-ttu-id="b90b3-114">Das Gerät wird vom Exchange-Server verwaltet.</span><span class="sxs-lookup"><span data-stu-id="b90b3-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="b90b3-115">MDM</span><span class="sxs-lookup"><span data-stu-id="b90b3-115">mdm</span></span>|<span data-ttu-id="b90b3-116">2</span><span class="sxs-lookup"><span data-stu-id="b90b3-116">2</span></span>|<span data-ttu-id="b90b3-117">Das Gerät wird durch Intune MDM verwaltet.</span><span class="sxs-lookup"><span data-stu-id="b90b3-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="b90b3-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="b90b3-118">easMdm</span></span>|<span data-ttu-id="b90b3-119">3</span><span class="sxs-lookup"><span data-stu-id="b90b3-119">3</span></span>|<span data-ttu-id="b90b3-120">Das Gerät wird von Exchange Server und Intune MDM verwaltet.</span><span class="sxs-lookup"><span data-stu-id="b90b3-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="b90b3-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="b90b3-121">intuneClient</span></span>|<span data-ttu-id="b90b3-122">4</span><span class="sxs-lookup"><span data-stu-id="b90b3-122">4</span></span>|<span data-ttu-id="b90b3-123">Intune Client verwaltet.</span><span class="sxs-lookup"><span data-stu-id="b90b3-123">Intune client managed.</span></span>|
|<span data-ttu-id="b90b3-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="b90b3-124">easIntuneClient</span></span>|<span data-ttu-id="b90b3-125">5</span><span class="sxs-lookup"><span data-stu-id="b90b3-125">5</span></span>|<span data-ttu-id="b90b3-126">Das Gerät ist EAS Intune-Client und zwei verwaltet.</span><span class="sxs-lookup"><span data-stu-id="b90b3-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="b90b3-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="b90b3-127">configurationManagerClient</span></span>|<span data-ttu-id="b90b3-128">8</span><span class="sxs-lookup"><span data-stu-id="b90b3-128">8</span></span>|<span data-ttu-id="b90b3-129">Das Gerät wird vom Konfigurations-Manager verwaltet.</span><span class="sxs-lookup"><span data-stu-id="b90b3-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="b90b3-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="b90b3-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="b90b3-131">10</span><span class="sxs-lookup"><span data-stu-id="b90b3-131">10</span></span>|<span data-ttu-id="b90b3-132">Das Gerät wird vom Konfigurations-Manager und MDM verwaltet.</span><span class="sxs-lookup"><span data-stu-id="b90b3-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="b90b3-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="b90b3-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="b90b3-134">11</span><span class="sxs-lookup"><span data-stu-id="b90b3-134">11</span></span>|<span data-ttu-id="b90b3-135">Das Gerät wird vom Konfigurations-Manager, MDM und Eas verwaltet.</span><span class="sxs-lookup"><span data-stu-id="b90b3-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="b90b3-136">unknown</span><span class="sxs-lookup"><span data-stu-id="b90b3-136">unknown</span></span>|<span data-ttu-id="b90b3-137">16</span><span class="sxs-lookup"><span data-stu-id="b90b3-137">16</span></span>|<span data-ttu-id="b90b3-138">Unbekannte Management Agent-Typ.</span><span class="sxs-lookup"><span data-stu-id="b90b3-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="b90b3-139">jamf</span><span class="sxs-lookup"><span data-stu-id="b90b3-139">jamf</span></span>|<span data-ttu-id="b90b3-140">32</span><span class="sxs-lookup"><span data-stu-id="b90b3-140">32</span></span>|<span data-ttu-id="b90b3-141">Das Gerätattribute werden aus Jamf abgerufen.</span><span class="sxs-lookup"><span data-stu-id="b90b3-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="b90b3-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="b90b3-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="b90b3-143">64</span><span class="sxs-lookup"><span data-stu-id="b90b3-143">64</span></span>|<span data-ttu-id="b90b3-144">Das Gerät wird von Google CloudDPC verwaltet.</span><span class="sxs-lookup"><span data-stu-id="b90b3-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="b90b3-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="b90b3-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="b90b3-146">258</span><span class="sxs-lookup"><span data-stu-id="b90b3-146">258</span></span>|<span data-ttu-id="b90b3-147">Dieses Gerät wird von Microsoft 365 über Intune verwaltet.</span><span class="sxs-lookup"><span data-stu-id="b90b3-147">This device is managed by Microsoft 365 through Intune.</span></span>|





