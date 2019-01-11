---
title: DeviceComplianceActionType Enum-Typ
description: Geplante Aktion Typ Enum
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e2b89dbdaa3e67918b1b0c3e76eb6638e492994c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881872"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="bb63f-103">DeviceComplianceActionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="bb63f-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="bb63f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bb63f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb63f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bb63f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb63f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bb63f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb63f-107">Geplante Aktion Typ Enum</span><span class="sxs-lookup"><span data-stu-id="bb63f-107">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="bb63f-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="bb63f-108">Members</span></span>
|<span data-ttu-id="bb63f-109">Element</span><span class="sxs-lookup"><span data-stu-id="bb63f-109">Member</span></span>|<span data-ttu-id="bb63f-110">Wert</span><span class="sxs-lookup"><span data-stu-id="bb63f-110">Value</span></span>|<span data-ttu-id="bb63f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb63f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb63f-112">noAction</span><span class="sxs-lookup"><span data-stu-id="bb63f-112">noAction</span></span>|<span data-ttu-id="bb63f-113">0</span><span class="sxs-lookup"><span data-stu-id="bb63f-113">0</span></span>|<span data-ttu-id="bb63f-114">Keine Aktion</span><span class="sxs-lookup"><span data-stu-id="bb63f-114">No Action</span></span>|
|<span data-ttu-id="bb63f-115">Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="bb63f-115">notification</span></span>|<span data-ttu-id="bb63f-116">1</span><span class="sxs-lookup"><span data-stu-id="bb63f-116">1</span></span>|<span data-ttu-id="bb63f-117">Benachrichtigung senden</span><span class="sxs-lookup"><span data-stu-id="bb63f-117">Send Notification</span></span>|
|<span data-ttu-id="bb63f-118">Blockieren</span><span class="sxs-lookup"><span data-stu-id="bb63f-118">block</span></span>|<span data-ttu-id="bb63f-119">2</span><span class="sxs-lookup"><span data-stu-id="bb63f-119">2</span></span>|<span data-ttu-id="bb63f-120">Das Gerät im AAD blockieren</span><span class="sxs-lookup"><span data-stu-id="bb63f-120">Block the device in AAD</span></span>|
|<span data-ttu-id="bb63f-121">Zurückziehen</span><span class="sxs-lookup"><span data-stu-id="bb63f-121">retire</span></span>|<span data-ttu-id="bb63f-122">3</span><span class="sxs-lookup"><span data-stu-id="bb63f-122">3</span></span>|<span data-ttu-id="bb63f-123">Deaktivieren Sie das Gerät</span><span class="sxs-lookup"><span data-stu-id="bb63f-123">Retire the device</span></span>|
|<span data-ttu-id="bb63f-124">Wischen</span><span class="sxs-lookup"><span data-stu-id="bb63f-124">wipe</span></span>|<span data-ttu-id="bb63f-125">4</span><span class="sxs-lookup"><span data-stu-id="bb63f-125">4</span></span>|<span data-ttu-id="bb63f-126">Bereinigen des Geräts</span><span class="sxs-lookup"><span data-stu-id="bb63f-126">Wipe the device</span></span>|
|<span data-ttu-id="bb63f-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="bb63f-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="bb63f-128">5</span><span class="sxs-lookup"><span data-stu-id="bb63f-128">5</span></span>|<span data-ttu-id="bb63f-129">Ressource Access Profile vom Gerät zu entfernen</span><span class="sxs-lookup"><span data-stu-id="bb63f-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="bb63f-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="bb63f-130">pushNotification</span></span>|<span data-ttu-id="bb63f-131">9</span><span class="sxs-lookup"><span data-stu-id="bb63f-131">9</span></span>|<span data-ttu-id="bb63f-132">Push-Benachrichtigung an Gerät senden</span><span class="sxs-lookup"><span data-stu-id="bb63f-132">Send push notification to device</span></span>|
|<span data-ttu-id="bb63f-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="bb63f-133">remoteLock</span></span>|<span data-ttu-id="bb63f-134">10</span><span class="sxs-lookup"><span data-stu-id="bb63f-134">10</span></span>|<span data-ttu-id="bb63f-135">Das Gerät Remote Sperren</span><span class="sxs-lookup"><span data-stu-id="bb63f-135">Remotely lock the device</span></span>|





