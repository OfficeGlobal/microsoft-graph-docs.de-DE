---
title: DeviceManagementSubscriptionState Enum-Typ
description: Status des Abonnements bei der Lösung für Mobilgeräteverwaltung des Mandanten.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a063252dcd3b65d85728550dd9ab616435a73472
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848370"
---
# <a name="devicemanagementsubscriptionstate-enum-type"></a><span data-ttu-id="d1a1c-103">DeviceManagementSubscriptionState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="d1a1c-103">deviceManagementSubscriptionState enum type</span></span>

> <span data-ttu-id="d1a1c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d1a1c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1a1c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d1a1c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1a1c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d1a1c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1a1c-107">Status des Abonnements bei der Lösung für Mobilgeräteverwaltung des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d1a1c-107">Tenant mobile device management subscription state.</span></span>
## <a name="members"></a><span data-ttu-id="d1a1c-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="d1a1c-108">Members</span></span>
|<span data-ttu-id="d1a1c-109">Element</span><span class="sxs-lookup"><span data-stu-id="d1a1c-109">Member</span></span>|<span data-ttu-id="d1a1c-110">Wert</span><span class="sxs-lookup"><span data-stu-id="d1a1c-110">Value</span></span>|<span data-ttu-id="d1a1c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1a1c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1a1c-112">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="d1a1c-112">pending</span></span>|<span data-ttu-id="d1a1c-113">0</span><span class="sxs-lookup"><span data-stu-id="d1a1c-113">0</span></span>|<span data-ttu-id="d1a1c-114">Ausstehend</span><span class="sxs-lookup"><span data-stu-id="d1a1c-114">Pending</span></span>|
|<span data-ttu-id="d1a1c-115">aktive</span><span class="sxs-lookup"><span data-stu-id="d1a1c-115">active</span></span>|<span data-ttu-id="d1a1c-116">1</span><span class="sxs-lookup"><span data-stu-id="d1a1c-116">1</span></span>|<span data-ttu-id="d1a1c-117">Active</span><span class="sxs-lookup"><span data-stu-id="d1a1c-117">Active</span></span>|
|<span data-ttu-id="d1a1c-118">warning</span><span class="sxs-lookup"><span data-stu-id="d1a1c-118">warning</span></span>|<span data-ttu-id="d1a1c-119">2</span><span class="sxs-lookup"><span data-stu-id="d1a1c-119">2</span></span>|<span data-ttu-id="d1a1c-120">Warnung</span><span class="sxs-lookup"><span data-stu-id="d1a1c-120">Warning</span></span>|
|<span data-ttu-id="d1a1c-121">deaktiviert</span><span class="sxs-lookup"><span data-stu-id="d1a1c-121">disabled</span></span>|<span data-ttu-id="d1a1c-122">3</span><span class="sxs-lookup"><span data-stu-id="d1a1c-122">3</span></span>|<span data-ttu-id="d1a1c-123">Deaktiviert</span><span class="sxs-lookup"><span data-stu-id="d1a1c-123">Disabled</span></span>|
|<span data-ttu-id="d1a1c-124">gelöscht</span><span class="sxs-lookup"><span data-stu-id="d1a1c-124">deleted</span></span>|<span data-ttu-id="d1a1c-125">4</span><span class="sxs-lookup"><span data-stu-id="d1a1c-125">4</span></span>|<span data-ttu-id="d1a1c-126">Gelöscht</span><span class="sxs-lookup"><span data-stu-id="d1a1c-126">Deleted</span></span>|
|<span data-ttu-id="d1a1c-127">gesperrt</span><span class="sxs-lookup"><span data-stu-id="d1a1c-127">blocked</span></span>|<span data-ttu-id="d1a1c-128">5</span><span class="sxs-lookup"><span data-stu-id="d1a1c-128">5</span></span>|<span data-ttu-id="d1a1c-129">Gesperrt</span><span class="sxs-lookup"><span data-stu-id="d1a1c-129">Blocked</span></span>|
|<span data-ttu-id="d1a1c-130">lockedOut</span><span class="sxs-lookup"><span data-stu-id="d1a1c-130">lockedOut</span></span>|<span data-ttu-id="d1a1c-131">8</span><span class="sxs-lookup"><span data-stu-id="d1a1c-131">8</span></span>|<span data-ttu-id="d1a1c-132">LockedOut</span><span class="sxs-lookup"><span data-stu-id="d1a1c-132">LockedOut</span></span>|





