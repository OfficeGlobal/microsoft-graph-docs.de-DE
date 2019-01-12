---
title: DeviceComplianceActionType Enum-Typ
description: Geplante Aktion Typ Enum
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1856847cb8a8ecf48ee6d13067bd24515326d89
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973209"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="6041a-103">DeviceComplianceActionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="6041a-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="6041a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6041a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6041a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6041a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6041a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6041a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6041a-107">Geplante Aktion Typ Enum</span><span class="sxs-lookup"><span data-stu-id="6041a-107">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="6041a-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="6041a-108">Members</span></span>
|<span data-ttu-id="6041a-109">Element</span><span class="sxs-lookup"><span data-stu-id="6041a-109">Member</span></span>|<span data-ttu-id="6041a-110">Wert</span><span class="sxs-lookup"><span data-stu-id="6041a-110">Value</span></span>|<span data-ttu-id="6041a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6041a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6041a-112">noAction</span><span class="sxs-lookup"><span data-stu-id="6041a-112">noAction</span></span>|<span data-ttu-id="6041a-113">0</span><span class="sxs-lookup"><span data-stu-id="6041a-113">0</span></span>|<span data-ttu-id="6041a-114">Keine Aktion</span><span class="sxs-lookup"><span data-stu-id="6041a-114">No Action</span></span>|
|<span data-ttu-id="6041a-115">Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="6041a-115">notification</span></span>|<span data-ttu-id="6041a-116">1</span><span class="sxs-lookup"><span data-stu-id="6041a-116">1</span></span>|<span data-ttu-id="6041a-117">Benachrichtigung senden</span><span class="sxs-lookup"><span data-stu-id="6041a-117">Send Notification</span></span>|
|<span data-ttu-id="6041a-118">Blockieren</span><span class="sxs-lookup"><span data-stu-id="6041a-118">block</span></span>|<span data-ttu-id="6041a-119">2</span><span class="sxs-lookup"><span data-stu-id="6041a-119">2</span></span>|<span data-ttu-id="6041a-120">Das Gerät im AAD blockieren</span><span class="sxs-lookup"><span data-stu-id="6041a-120">Block the device in AAD</span></span>|
|<span data-ttu-id="6041a-121">Zurückziehen</span><span class="sxs-lookup"><span data-stu-id="6041a-121">retire</span></span>|<span data-ttu-id="6041a-122">3</span><span class="sxs-lookup"><span data-stu-id="6041a-122">3</span></span>|<span data-ttu-id="6041a-123">Deaktivieren Sie das Gerät</span><span class="sxs-lookup"><span data-stu-id="6041a-123">Retire the device</span></span>|
|<span data-ttu-id="6041a-124">Wischen</span><span class="sxs-lookup"><span data-stu-id="6041a-124">wipe</span></span>|<span data-ttu-id="6041a-125">4</span><span class="sxs-lookup"><span data-stu-id="6041a-125">4</span></span>|<span data-ttu-id="6041a-126">Bereinigen des Geräts</span><span class="sxs-lookup"><span data-stu-id="6041a-126">Wipe the device</span></span>|
|<span data-ttu-id="6041a-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="6041a-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="6041a-128">5</span><span class="sxs-lookup"><span data-stu-id="6041a-128">5</span></span>|<span data-ttu-id="6041a-129">Ressource Access Profile vom Gerät zu entfernen</span><span class="sxs-lookup"><span data-stu-id="6041a-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="6041a-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="6041a-130">pushNotification</span></span>|<span data-ttu-id="6041a-131">9</span><span class="sxs-lookup"><span data-stu-id="6041a-131">9</span></span>|<span data-ttu-id="6041a-132">Push-Benachrichtigung an Gerät senden</span><span class="sxs-lookup"><span data-stu-id="6041a-132">Send push notification to device</span></span>|
|<span data-ttu-id="6041a-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="6041a-133">remoteLock</span></span>|<span data-ttu-id="6041a-134">10</span><span class="sxs-lookup"><span data-stu-id="6041a-134">10</span></span>|<span data-ttu-id="6041a-135">Das Gerät Remote Sperren</span><span class="sxs-lookup"><span data-stu-id="6041a-135">Remotely lock the device</span></span>|





