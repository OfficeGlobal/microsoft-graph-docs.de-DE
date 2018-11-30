---
title: DeviceComplianceActionType Enum-Typ
description: Geplante Aktion Typ Enum
ms.openlocfilehash: 98e54f163663cc041a3e3c31123504c051884309
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061205"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="107aa-103">DeviceComplianceActionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="107aa-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="107aa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="107aa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="107aa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="107aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="107aa-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="107aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="107aa-107">Geplante Aktion Typ Enum</span><span class="sxs-lookup"><span data-stu-id="107aa-107">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="107aa-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="107aa-108">Members</span></span>
|<span data-ttu-id="107aa-109">Element</span><span class="sxs-lookup"><span data-stu-id="107aa-109">Member</span></span>|<span data-ttu-id="107aa-110">Wert</span><span class="sxs-lookup"><span data-stu-id="107aa-110">Value</span></span>|<span data-ttu-id="107aa-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="107aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="107aa-112">noAction</span><span class="sxs-lookup"><span data-stu-id="107aa-112">noAction</span></span>|<span data-ttu-id="107aa-113">0</span><span class="sxs-lookup"><span data-stu-id="107aa-113">0</span></span>|<span data-ttu-id="107aa-114">Keine Aktion</span><span class="sxs-lookup"><span data-stu-id="107aa-114">No Action</span></span>|
|<span data-ttu-id="107aa-115">Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="107aa-115">notification</span></span>|<span data-ttu-id="107aa-116">1</span><span class="sxs-lookup"><span data-stu-id="107aa-116">1</span></span>|<span data-ttu-id="107aa-117">Benachrichtigung senden</span><span class="sxs-lookup"><span data-stu-id="107aa-117">Send Notification</span></span>|
|<span data-ttu-id="107aa-118">Blockieren</span><span class="sxs-lookup"><span data-stu-id="107aa-118">block</span></span>|<span data-ttu-id="107aa-119">2</span><span class="sxs-lookup"><span data-stu-id="107aa-119">2</span></span>|<span data-ttu-id="107aa-120">Das Gerät im AAD blockieren</span><span class="sxs-lookup"><span data-stu-id="107aa-120">Block the device in AAD</span></span>|
|<span data-ttu-id="107aa-121">Zurückziehen</span><span class="sxs-lookup"><span data-stu-id="107aa-121">retire</span></span>|<span data-ttu-id="107aa-122">3</span><span class="sxs-lookup"><span data-stu-id="107aa-122">3</span></span>|<span data-ttu-id="107aa-123">Deaktivieren Sie das Gerät</span><span class="sxs-lookup"><span data-stu-id="107aa-123">Retire the device</span></span>|
|<span data-ttu-id="107aa-124">Wischen</span><span class="sxs-lookup"><span data-stu-id="107aa-124">wipe</span></span>|<span data-ttu-id="107aa-125">4</span><span class="sxs-lookup"><span data-stu-id="107aa-125">4</span></span>|<span data-ttu-id="107aa-126">Bereinigen des Geräts</span><span class="sxs-lookup"><span data-stu-id="107aa-126">Wipe the device</span></span>|
|<span data-ttu-id="107aa-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="107aa-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="107aa-128">5</span><span class="sxs-lookup"><span data-stu-id="107aa-128">5</span></span>|<span data-ttu-id="107aa-129">Ressource Access Profile vom Gerät zu entfernen</span><span class="sxs-lookup"><span data-stu-id="107aa-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="107aa-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="107aa-130">pushNotification</span></span>|<span data-ttu-id="107aa-131">9</span><span class="sxs-lookup"><span data-stu-id="107aa-131">9</span></span>|<span data-ttu-id="107aa-132">Push-Benachrichtigung an Gerät senden</span><span class="sxs-lookup"><span data-stu-id="107aa-132">Send push notification to device</span></span>|
|<span data-ttu-id="107aa-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="107aa-133">remoteLock</span></span>|<span data-ttu-id="107aa-134">10</span><span class="sxs-lookup"><span data-stu-id="107aa-134">10</span></span>|<span data-ttu-id="107aa-135">Das Gerät Remote Sperren</span><span class="sxs-lookup"><span data-stu-id="107aa-135">Remotely lock the device</span></span>|





