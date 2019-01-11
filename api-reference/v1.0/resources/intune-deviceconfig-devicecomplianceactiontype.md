---
title: DeviceComplianceActionType Enum-Typ
description: Geplante Aktion Typ Enum
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 92e43378f119a5e1a10604babb5ad23b2dfddf3b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851436"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="3b651-103">DeviceComplianceActionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="3b651-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="3b651-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3b651-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b651-105">Geplante Aktion Typ Enum</span><span class="sxs-lookup"><span data-stu-id="3b651-105">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="3b651-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="3b651-106">Members</span></span>
|<span data-ttu-id="3b651-107">Element</span><span class="sxs-lookup"><span data-stu-id="3b651-107">Member</span></span>|<span data-ttu-id="3b651-108">Wert</span><span class="sxs-lookup"><span data-stu-id="3b651-108">Value</span></span>|<span data-ttu-id="3b651-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b651-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b651-110">noAction</span><span class="sxs-lookup"><span data-stu-id="3b651-110">noAction</span></span>|<span data-ttu-id="3b651-111">0</span><span class="sxs-lookup"><span data-stu-id="3b651-111">0</span></span>|<span data-ttu-id="3b651-112">Keine Aktion</span><span class="sxs-lookup"><span data-stu-id="3b651-112">No Action</span></span>|
|<span data-ttu-id="3b651-113">Benachrichtigung</span><span class="sxs-lookup"><span data-stu-id="3b651-113">notification</span></span>|<span data-ttu-id="3b651-114">1</span><span class="sxs-lookup"><span data-stu-id="3b651-114">1</span></span>|<span data-ttu-id="3b651-115">Benachrichtigung senden</span><span class="sxs-lookup"><span data-stu-id="3b651-115">Send Notification</span></span>|
|<span data-ttu-id="3b651-116">Blockieren</span><span class="sxs-lookup"><span data-stu-id="3b651-116">block</span></span>|<span data-ttu-id="3b651-117">2</span><span class="sxs-lookup"><span data-stu-id="3b651-117">2</span></span>|<span data-ttu-id="3b651-118">Das Gerät im AAD blockieren</span><span class="sxs-lookup"><span data-stu-id="3b651-118">Block the device in AAD</span></span>|
|<span data-ttu-id="3b651-119">Zurückziehen</span><span class="sxs-lookup"><span data-stu-id="3b651-119">retire</span></span>|<span data-ttu-id="3b651-120">3</span><span class="sxs-lookup"><span data-stu-id="3b651-120">3</span></span>|<span data-ttu-id="3b651-121">Deaktivieren Sie das Gerät</span><span class="sxs-lookup"><span data-stu-id="3b651-121">Retire the device</span></span>|
|<span data-ttu-id="3b651-122">Wischen</span><span class="sxs-lookup"><span data-stu-id="3b651-122">wipe</span></span>|<span data-ttu-id="3b651-123">4</span><span class="sxs-lookup"><span data-stu-id="3b651-123">4</span></span>|<span data-ttu-id="3b651-124">Bereinigen des Geräts</span><span class="sxs-lookup"><span data-stu-id="3b651-124">Wipe the device</span></span>|
|<span data-ttu-id="3b651-125">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="3b651-125">removeResourceAccessProfiles</span></span>|<span data-ttu-id="3b651-126">5</span><span class="sxs-lookup"><span data-stu-id="3b651-126">5</span></span>|<span data-ttu-id="3b651-127">Ressource Access Profile vom Gerät zu entfernen</span><span class="sxs-lookup"><span data-stu-id="3b651-127">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="3b651-128">pushNotification</span><span class="sxs-lookup"><span data-stu-id="3b651-128">pushNotification</span></span>|<span data-ttu-id="3b651-129">9</span><span class="sxs-lookup"><span data-stu-id="3b651-129">9</span></span>|<span data-ttu-id="3b651-130">Push-Benachrichtigung an Gerät senden</span><span class="sxs-lookup"><span data-stu-id="3b651-130">Send push notification to device</span></span>|



