---
title: deviceComplianceActionType-Enumerationstyp
description: Enum für geplante Aktionstypen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d824f579787bf24cc56704a1c8a9df280d969809
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173507"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="401a2-103">deviceComplianceActionType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="401a2-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="401a2-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="401a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="401a2-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="401a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="401a2-106">Enum für geplante Aktionstypen</span><span class="sxs-lookup"><span data-stu-id="401a2-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="401a2-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="401a2-107">Members</span></span>
|<span data-ttu-id="401a2-108">Element</span><span class="sxs-lookup"><span data-stu-id="401a2-108">Member</span></span>|<span data-ttu-id="401a2-109">Wert</span><span class="sxs-lookup"><span data-stu-id="401a2-109">Value</span></span>|<span data-ttu-id="401a2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="401a2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="401a2-111">noAction</span><span class="sxs-lookup"><span data-stu-id="401a2-111">noAction</span></span>|<span data-ttu-id="401a2-112">0</span><span class="sxs-lookup"><span data-stu-id="401a2-112">0</span></span>|<span data-ttu-id="401a2-113">Keine Aktion</span><span class="sxs-lookup"><span data-stu-id="401a2-113">No Action</span></span>|
|<span data-ttu-id="401a2-114">Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="401a2-114">notification</span></span>|<span data-ttu-id="401a2-115">1</span><span class="sxs-lookup"><span data-stu-id="401a2-115">1</span></span>|<span data-ttu-id="401a2-116">Benachrichtigung senden</span><span class="sxs-lookup"><span data-stu-id="401a2-116">Send Notification</span></span>|
|<span data-ttu-id="401a2-117">Block</span><span class="sxs-lookup"><span data-stu-id="401a2-117">block</span></span>|<span data-ttu-id="401a2-118">2</span><span class="sxs-lookup"><span data-stu-id="401a2-118">2</span></span>|<span data-ttu-id="401a2-119">Blockieren des Geräts in AAD</span><span class="sxs-lookup"><span data-stu-id="401a2-119">Block the device in AAD</span></span>|
|<span data-ttu-id="401a2-120">zurückziehen</span><span class="sxs-lookup"><span data-stu-id="401a2-120">retire</span></span>|<span data-ttu-id="401a2-121">3</span><span class="sxs-lookup"><span data-stu-id="401a2-121">3</span></span>|<span data-ttu-id="401a2-122">Zurückziehen des Geräts</span><span class="sxs-lookup"><span data-stu-id="401a2-122">Retire the device</span></span>|
|<span data-ttu-id="401a2-123">Zurücksetzung</span><span class="sxs-lookup"><span data-stu-id="401a2-123">wipe</span></span>|<span data-ttu-id="401a2-124">4</span><span class="sxs-lookup"><span data-stu-id="401a2-124">4</span></span>|<span data-ttu-id="401a2-125">Wischen Sie das Gerät ab.</span><span class="sxs-lookup"><span data-stu-id="401a2-125">Wipe the device</span></span>|
|<span data-ttu-id="401a2-126">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="401a2-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="401a2-127">5</span><span class="sxs-lookup"><span data-stu-id="401a2-127">5</span></span>|<span data-ttu-id="401a2-128">Entfernen von Ressourcenzugriffs Profilen vom Gerät</span><span class="sxs-lookup"><span data-stu-id="401a2-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="401a2-129">pushNotification</span><span class="sxs-lookup"><span data-stu-id="401a2-129">pushNotification</span></span>|<span data-ttu-id="401a2-130">9</span><span class="sxs-lookup"><span data-stu-id="401a2-130">9</span></span>|<span data-ttu-id="401a2-131">Push-Benachrichtigung an Gerät senden</span><span class="sxs-lookup"><span data-stu-id="401a2-131">Send push notification to device</span></span>|
|<span data-ttu-id="401a2-132">Remote Lock</span><span class="sxs-lookup"><span data-stu-id="401a2-132">remoteLock</span></span>|<span data-ttu-id="401a2-133">10</span><span class="sxs-lookup"><span data-stu-id="401a2-133">10</span></span>|<span data-ttu-id="401a2-134">Remote Sperre des Geräts</span><span class="sxs-lookup"><span data-stu-id="401a2-134">Remotely lock the device</span></span>|




