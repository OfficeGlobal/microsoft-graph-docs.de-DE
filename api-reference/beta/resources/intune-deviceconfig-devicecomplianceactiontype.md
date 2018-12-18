---
title: DeviceComplianceActionType Enum-Typ
description: Geplante Aktion Typ Enum
author: tfitzmac
ms.openlocfilehash: 9fd0a8bd045ad04fe0acf55f899e693d7fcce5d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335686"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="f61fe-103">DeviceComplianceActionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="f61fe-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="f61fe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f61fe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f61fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f61fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f61fe-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f61fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f61fe-107">Geplante Aktion Typ Enum</span><span class="sxs-lookup"><span data-stu-id="f61fe-107">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="f61fe-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="f61fe-108">Members</span></span>
|<span data-ttu-id="f61fe-109">Member</span><span class="sxs-lookup"><span data-stu-id="f61fe-109">Member</span></span>|<span data-ttu-id="f61fe-110">Wert</span><span class="sxs-lookup"><span data-stu-id="f61fe-110">Value</span></span>|<span data-ttu-id="f61fe-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f61fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f61fe-112">noAction</span><span class="sxs-lookup"><span data-stu-id="f61fe-112">noAction</span></span>|<span data-ttu-id="f61fe-113">0</span><span class="sxs-lookup"><span data-stu-id="f61fe-113">0</span></span>|<span data-ttu-id="f61fe-114">Keine Aktion</span><span class="sxs-lookup"><span data-stu-id="f61fe-114">No Action</span></span>|
|<span data-ttu-id="f61fe-115">Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="f61fe-115">notification</span></span>|<span data-ttu-id="f61fe-116">1</span><span class="sxs-lookup"><span data-stu-id="f61fe-116">1</span></span>|<span data-ttu-id="f61fe-117">Benachrichtigung senden</span><span class="sxs-lookup"><span data-stu-id="f61fe-117">Send Notification</span></span>|
|<span data-ttu-id="f61fe-118">Blockieren</span><span class="sxs-lookup"><span data-stu-id="f61fe-118">block</span></span>|<span data-ttu-id="f61fe-119">2</span><span class="sxs-lookup"><span data-stu-id="f61fe-119">2</span></span>|<span data-ttu-id="f61fe-120">Das Gerät im AAD blockieren</span><span class="sxs-lookup"><span data-stu-id="f61fe-120">Block the device in AAD</span></span>|
|<span data-ttu-id="f61fe-121">Zurückziehen</span><span class="sxs-lookup"><span data-stu-id="f61fe-121">retire</span></span>|<span data-ttu-id="f61fe-122">3</span><span class="sxs-lookup"><span data-stu-id="f61fe-122">3</span></span>|<span data-ttu-id="f61fe-123">Deaktivieren Sie das Gerät</span><span class="sxs-lookup"><span data-stu-id="f61fe-123">Retire the device</span></span>|
|<span data-ttu-id="f61fe-124">Wischen</span><span class="sxs-lookup"><span data-stu-id="f61fe-124">wipe</span></span>|<span data-ttu-id="f61fe-125">4</span><span class="sxs-lookup"><span data-stu-id="f61fe-125">4</span></span>|<span data-ttu-id="f61fe-126">Bereinigen des Geräts</span><span class="sxs-lookup"><span data-stu-id="f61fe-126">Wipe the device</span></span>|
|<span data-ttu-id="f61fe-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="f61fe-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="f61fe-128">5</span><span class="sxs-lookup"><span data-stu-id="f61fe-128">5</span></span>|<span data-ttu-id="f61fe-129">Ressource Access Profile vom Gerät zu entfernen</span><span class="sxs-lookup"><span data-stu-id="f61fe-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="f61fe-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="f61fe-130">pushNotification</span></span>|<span data-ttu-id="f61fe-131">9</span><span class="sxs-lookup"><span data-stu-id="f61fe-131">9</span></span>|<span data-ttu-id="f61fe-132">Push-Benachrichtigung an Gerät senden</span><span class="sxs-lookup"><span data-stu-id="f61fe-132">Send push notification to device</span></span>|
|<span data-ttu-id="f61fe-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="f61fe-133">remoteLock</span></span>|<span data-ttu-id="f61fe-134">10</span><span class="sxs-lookup"><span data-stu-id="f61fe-134">10</span></span>|<span data-ttu-id="f61fe-135">Das Gerät Remote Sperren</span><span class="sxs-lookup"><span data-stu-id="f61fe-135">Remotely lock the device</span></span>|





