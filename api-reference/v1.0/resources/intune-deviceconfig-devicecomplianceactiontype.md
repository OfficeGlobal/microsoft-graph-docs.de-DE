---
title: DeviceComplianceActionType Enum-Typ
description: Geplante Aktion Typ Enum
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8d725213790260ece51c02bb81f2394fc8602095
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917342"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="6a79c-103">DeviceComplianceActionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="6a79c-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="6a79c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6a79c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a79c-105">Geplante Aktion Typ Enum</span><span class="sxs-lookup"><span data-stu-id="6a79c-105">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="6a79c-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="6a79c-106">Members</span></span>
|<span data-ttu-id="6a79c-107">Element</span><span class="sxs-lookup"><span data-stu-id="6a79c-107">Member</span></span>|<span data-ttu-id="6a79c-108">Wert</span><span class="sxs-lookup"><span data-stu-id="6a79c-108">Value</span></span>|<span data-ttu-id="6a79c-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a79c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a79c-110">noAction</span><span class="sxs-lookup"><span data-stu-id="6a79c-110">noAction</span></span>|<span data-ttu-id="6a79c-111">0</span><span class="sxs-lookup"><span data-stu-id="6a79c-111">0</span></span>|<span data-ttu-id="6a79c-112">Keine Aktion</span><span class="sxs-lookup"><span data-stu-id="6a79c-112">No Action</span></span>|
|<span data-ttu-id="6a79c-113">Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="6a79c-113">notification</span></span>|<span data-ttu-id="6a79c-114">1</span><span class="sxs-lookup"><span data-stu-id="6a79c-114">1</span></span>|<span data-ttu-id="6a79c-115">Benachrichtigung senden</span><span class="sxs-lookup"><span data-stu-id="6a79c-115">Send Notification</span></span>|
|<span data-ttu-id="6a79c-116">Blockieren</span><span class="sxs-lookup"><span data-stu-id="6a79c-116">block</span></span>|<span data-ttu-id="6a79c-117">2</span><span class="sxs-lookup"><span data-stu-id="6a79c-117">2</span></span>|<span data-ttu-id="6a79c-118">Das Gerät im AAD blockieren</span><span class="sxs-lookup"><span data-stu-id="6a79c-118">Block the device in AAD</span></span>|
|<span data-ttu-id="6a79c-119">Zurückziehen</span><span class="sxs-lookup"><span data-stu-id="6a79c-119">retire</span></span>|<span data-ttu-id="6a79c-120">3</span><span class="sxs-lookup"><span data-stu-id="6a79c-120">3</span></span>|<span data-ttu-id="6a79c-121">Deaktivieren Sie das Gerät</span><span class="sxs-lookup"><span data-stu-id="6a79c-121">Retire the device</span></span>|
|<span data-ttu-id="6a79c-122">Wischen</span><span class="sxs-lookup"><span data-stu-id="6a79c-122">wipe</span></span>|<span data-ttu-id="6a79c-123">4</span><span class="sxs-lookup"><span data-stu-id="6a79c-123">4</span></span>|<span data-ttu-id="6a79c-124">Bereinigen des Geräts</span><span class="sxs-lookup"><span data-stu-id="6a79c-124">Wipe the device</span></span>|
|<span data-ttu-id="6a79c-125">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="6a79c-125">removeResourceAccessProfiles</span></span>|<span data-ttu-id="6a79c-126">5</span><span class="sxs-lookup"><span data-stu-id="6a79c-126">5</span></span>|<span data-ttu-id="6a79c-127">Ressource Access Profile vom Gerät zu entfernen</span><span class="sxs-lookup"><span data-stu-id="6a79c-127">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="6a79c-128">pushNotification</span><span class="sxs-lookup"><span data-stu-id="6a79c-128">pushNotification</span></span>|<span data-ttu-id="6a79c-129">9</span><span class="sxs-lookup"><span data-stu-id="6a79c-129">9</span></span>|<span data-ttu-id="6a79c-130">Push-Benachrichtigung an Gerät senden</span><span class="sxs-lookup"><span data-stu-id="6a79c-130">Send push notification to device</span></span>|



