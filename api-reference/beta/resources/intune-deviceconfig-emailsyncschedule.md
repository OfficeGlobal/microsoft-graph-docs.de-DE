---
title: EmailSyncSchedule Enum-Typ
description: Mögliche Werte für e-Mail-Synchronisierungszeitplan.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9dc93bce19262d0b1aad1d1cc8f28ea4db56ce9f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924041"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="bbace-103">EmailSyncSchedule Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="bbace-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="bbace-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bbace-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbace-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bbace-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bbace-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bbace-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bbace-107">Mögliche Werte für e-Mail-Synchronisierungszeitplan.</span><span class="sxs-lookup"><span data-stu-id="bbace-107">Possible values for email sync schedule.</span></span>
## <a name="members"></a><span data-ttu-id="bbace-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="bbace-108">Members</span></span>
|<span data-ttu-id="bbace-109">Element</span><span class="sxs-lookup"><span data-stu-id="bbace-109">Member</span></span>|<span data-ttu-id="bbace-110">Wert</span><span class="sxs-lookup"><span data-stu-id="bbace-110">Value</span></span>|<span data-ttu-id="bbace-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bbace-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbace-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="bbace-112">userDefined</span></span>|<span data-ttu-id="bbace-113">0</span><span class="sxs-lookup"><span data-stu-id="bbace-113">0</span></span>|<span data-ttu-id="bbace-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="bbace-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="bbace-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="bbace-115">asMessagesArrive</span></span>|<span data-ttu-id="bbace-116">1</span><span class="sxs-lookup"><span data-stu-id="bbace-116">1</span></span>|<span data-ttu-id="bbace-117">Synchronisieren Sie wie Nachrichten eingehen.</span><span class="sxs-lookup"><span data-stu-id="bbace-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="bbace-118">Manuell</span><span class="sxs-lookup"><span data-stu-id="bbace-118">manual</span></span>|<span data-ttu-id="bbace-119">2</span><span class="sxs-lookup"><span data-stu-id="bbace-119">2</span></span>|<span data-ttu-id="bbace-120">Manuell synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="bbace-120">Sync manually.</span></span>|
|<span data-ttu-id="bbace-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="bbace-121">fifteenMinutes</span></span>|<span data-ttu-id="bbace-122">3</span><span class="sxs-lookup"><span data-stu-id="bbace-122">3</span></span>|<span data-ttu-id="bbace-123">Synchronisieren Sie alle 15 Minuten.</span><span class="sxs-lookup"><span data-stu-id="bbace-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="bbace-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="bbace-124">thirtyMinutes</span></span>|<span data-ttu-id="bbace-125">4</span><span class="sxs-lookup"><span data-stu-id="bbace-125">4</span></span>|<span data-ttu-id="bbace-126">Sync alle 30 Minuten.</span><span class="sxs-lookup"><span data-stu-id="bbace-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="bbace-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="bbace-127">sixtyMinutes</span></span>|<span data-ttu-id="bbace-128">5</span><span class="sxs-lookup"><span data-stu-id="bbace-128">5</span></span>|<span data-ttu-id="bbace-129">Sync alle 60 Minuten.</span><span class="sxs-lookup"><span data-stu-id="bbace-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="bbace-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="bbace-130">basedOnMyUsage</span></span>|<span data-ttu-id="bbace-131">6</span><span class="sxs-lookup"><span data-stu-id="bbace-131">6</span></span>|<span data-ttu-id="bbace-132">Die Synchronisierung basierend auf meine Verwendung.</span><span class="sxs-lookup"><span data-stu-id="bbace-132">Sync based on my usage.</span></span>|





