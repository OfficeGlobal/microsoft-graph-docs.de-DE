---
title: DeviceManagementSubscriptionState Enum-Typ
description: Status des Abonnements bei der Lösung für Mobilgeräteverwaltung des Mandanten.
author: tfitzmac
ms.openlocfilehash: 840614cad992fb057f8bd4a803a1fe9479a26be3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323611"
---
# <a name="devicemanagementsubscriptionstate-enum-type"></a><span data-ttu-id="fa5c8-103">DeviceManagementSubscriptionState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="fa5c8-103">deviceManagementSubscriptionState enum type</span></span>

> <span data-ttu-id="fa5c8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fa5c8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa5c8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa5c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa5c8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fa5c8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa5c8-107">Status des Abonnements bei der Lösung für Mobilgeräteverwaltung des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fa5c8-107">Tenant mobile device management subscription state.</span></span>
## <a name="members"></a><span data-ttu-id="fa5c8-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="fa5c8-108">Members</span></span>
|<span data-ttu-id="fa5c8-109">Member</span><span class="sxs-lookup"><span data-stu-id="fa5c8-109">Member</span></span>|<span data-ttu-id="fa5c8-110">Wert</span><span class="sxs-lookup"><span data-stu-id="fa5c8-110">Value</span></span>|<span data-ttu-id="fa5c8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa5c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa5c8-112">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="fa5c8-112">pending</span></span>|<span data-ttu-id="fa5c8-113">0</span><span class="sxs-lookup"><span data-stu-id="fa5c8-113">0</span></span>|<span data-ttu-id="fa5c8-114">Ausstehend</span><span class="sxs-lookup"><span data-stu-id="fa5c8-114">Pending</span></span>|
|<span data-ttu-id="fa5c8-115">aktive</span><span class="sxs-lookup"><span data-stu-id="fa5c8-115">active</span></span>|<span data-ttu-id="fa5c8-116">1</span><span class="sxs-lookup"><span data-stu-id="fa5c8-116">1</span></span>|<span data-ttu-id="fa5c8-117">Active</span><span class="sxs-lookup"><span data-stu-id="fa5c8-117">Active</span></span>|
|<span data-ttu-id="fa5c8-118">warning</span><span class="sxs-lookup"><span data-stu-id="fa5c8-118">warning</span></span>|<span data-ttu-id="fa5c8-119">2</span><span class="sxs-lookup"><span data-stu-id="fa5c8-119">2</span></span>|<span data-ttu-id="fa5c8-120">Warnung</span><span class="sxs-lookup"><span data-stu-id="fa5c8-120">Warning</span></span>|
|<span data-ttu-id="fa5c8-121">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="fa5c8-121">disabled</span></span>|<span data-ttu-id="fa5c8-122">3</span><span class="sxs-lookup"><span data-stu-id="fa5c8-122">3</span></span>|<span data-ttu-id="fa5c8-123">Deaktiviert</span><span class="sxs-lookup"><span data-stu-id="fa5c8-123">Disabled</span></span>|
|<span data-ttu-id="fa5c8-124">gelöscht</span><span class="sxs-lookup"><span data-stu-id="fa5c8-124">deleted</span></span>|<span data-ttu-id="fa5c8-125">4</span><span class="sxs-lookup"><span data-stu-id="fa5c8-125">4</span></span>|<span data-ttu-id="fa5c8-126">Gelöscht</span><span class="sxs-lookup"><span data-stu-id="fa5c8-126">Deleted</span></span>|
|<span data-ttu-id="fa5c8-127">gesperrt</span><span class="sxs-lookup"><span data-stu-id="fa5c8-127">blocked</span></span>|<span data-ttu-id="fa5c8-128">5</span><span class="sxs-lookup"><span data-stu-id="fa5c8-128">5</span></span>|<span data-ttu-id="fa5c8-129">Gesperrt</span><span class="sxs-lookup"><span data-stu-id="fa5c8-129">Blocked</span></span>|
|<span data-ttu-id="fa5c8-130">lockedOut</span><span class="sxs-lookup"><span data-stu-id="fa5c8-130">lockedOut</span></span>|<span data-ttu-id="fa5c8-131">8</span><span class="sxs-lookup"><span data-stu-id="fa5c8-131">8</span></span>|<span data-ttu-id="fa5c8-132">LockedOut</span><span class="sxs-lookup"><span data-stu-id="fa5c8-132">LockedOut</span></span>|





