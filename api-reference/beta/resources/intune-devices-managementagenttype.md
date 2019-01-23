---
title: ManagementAgentType Enum-Typ
description: Typ der Management Agent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9c42d4ea4a5114bc42966891e4cd60ea87ca303e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401005"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="42906-103">ManagementAgentType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="42906-103">managementAgentType enum type</span></span>

> <span data-ttu-id="42906-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="42906-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="42906-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="42906-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42906-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="42906-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42906-107">Typ der Management Agent.</span><span class="sxs-lookup"><span data-stu-id="42906-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="42906-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="42906-108">Members</span></span>
|<span data-ttu-id="42906-109">Member</span><span class="sxs-lookup"><span data-stu-id="42906-109">Member</span></span>|<span data-ttu-id="42906-110">Wert</span><span class="sxs-lookup"><span data-stu-id="42906-110">Value</span></span>|<span data-ttu-id="42906-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42906-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42906-112">EAS</span><span class="sxs-lookup"><span data-stu-id="42906-112">eas</span></span>|<span data-ttu-id="42906-113">1</span><span class="sxs-lookup"><span data-stu-id="42906-113">1</span></span>|<span data-ttu-id="42906-114">Das Gerät wird vom Exchange-Server verwaltet.</span><span class="sxs-lookup"><span data-stu-id="42906-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="42906-115">MDM</span><span class="sxs-lookup"><span data-stu-id="42906-115">mdm</span></span>|<span data-ttu-id="42906-116">2</span><span class="sxs-lookup"><span data-stu-id="42906-116">2</span></span>|<span data-ttu-id="42906-117">Das Gerät wird durch Intune MDM verwaltet.</span><span class="sxs-lookup"><span data-stu-id="42906-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="42906-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="42906-118">easMdm</span></span>|<span data-ttu-id="42906-119">3</span><span class="sxs-lookup"><span data-stu-id="42906-119">3</span></span>|<span data-ttu-id="42906-120">Das Gerät wird von Exchange Server und Intune MDM verwaltet.</span><span class="sxs-lookup"><span data-stu-id="42906-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="42906-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="42906-121">intuneClient</span></span>|<span data-ttu-id="42906-122">4</span><span class="sxs-lookup"><span data-stu-id="42906-122">4</span></span>|<span data-ttu-id="42906-123">Intune Client verwaltet.</span><span class="sxs-lookup"><span data-stu-id="42906-123">Intune client managed.</span></span>|
|<span data-ttu-id="42906-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="42906-124">easIntuneClient</span></span>|<span data-ttu-id="42906-125">5</span><span class="sxs-lookup"><span data-stu-id="42906-125">5</span></span>|<span data-ttu-id="42906-126">Das Gerät ist EAS Intune-Client und zwei verwaltet.</span><span class="sxs-lookup"><span data-stu-id="42906-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="42906-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="42906-127">configurationManagerClient</span></span>|<span data-ttu-id="42906-128">8</span><span class="sxs-lookup"><span data-stu-id="42906-128">8</span></span>|<span data-ttu-id="42906-129">Das Gerät wird vom Konfigurations-Manager verwaltet.</span><span class="sxs-lookup"><span data-stu-id="42906-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="42906-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="42906-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="42906-131">10</span><span class="sxs-lookup"><span data-stu-id="42906-131">10</span></span>|<span data-ttu-id="42906-132">Das Gerät wird vom Konfigurations-Manager und MDM verwaltet.</span><span class="sxs-lookup"><span data-stu-id="42906-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="42906-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="42906-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="42906-134">11</span><span class="sxs-lookup"><span data-stu-id="42906-134">11</span></span>|<span data-ttu-id="42906-135">Das Gerät wird vom Konfigurations-Manager, MDM und Eas verwaltet.</span><span class="sxs-lookup"><span data-stu-id="42906-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="42906-136">unknown</span><span class="sxs-lookup"><span data-stu-id="42906-136">unknown</span></span>|<span data-ttu-id="42906-137">16</span><span class="sxs-lookup"><span data-stu-id="42906-137">16</span></span>|<span data-ttu-id="42906-138">Unbekannte Management Agent-Typ.</span><span class="sxs-lookup"><span data-stu-id="42906-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="42906-139">jamf</span><span class="sxs-lookup"><span data-stu-id="42906-139">jamf</span></span>|<span data-ttu-id="42906-140">32</span><span class="sxs-lookup"><span data-stu-id="42906-140">32</span></span>|<span data-ttu-id="42906-141">Das Gerätattribute werden aus Jamf abgerufen.</span><span class="sxs-lookup"><span data-stu-id="42906-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="42906-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="42906-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="42906-143">64</span><span class="sxs-lookup"><span data-stu-id="42906-143">64</span></span>|<span data-ttu-id="42906-144">Das Gerät wird von Google CloudDPC verwaltet.</span><span class="sxs-lookup"><span data-stu-id="42906-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="42906-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="42906-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="42906-146">258</span><span class="sxs-lookup"><span data-stu-id="42906-146">258</span></span>|<span data-ttu-id="42906-147">Dieses Gerät wird von Microsoft 365 über Intune verwaltet.</span><span class="sxs-lookup"><span data-stu-id="42906-147">This device is managed by Microsoft 365 through Intune.</span></span>|




