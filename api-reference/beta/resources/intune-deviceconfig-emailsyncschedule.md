---
title: EmailSyncSchedule Enum-Typ
description: Mögliche Werte für e-Mail-Synchronisierungszeitplan.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 178cba9e226b7f20e3fd917145e7bbd06f6c3a1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838395"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="28c5f-103">EmailSyncSchedule Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="28c5f-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="28c5f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="28c5f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28c5f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="28c5f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28c5f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="28c5f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28c5f-107">Mögliche Werte für e-Mail-Synchronisierungszeitplan.</span><span class="sxs-lookup"><span data-stu-id="28c5f-107">Possible values for email sync schedule.</span></span>
## <a name="members"></a><span data-ttu-id="28c5f-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="28c5f-108">Members</span></span>
|<span data-ttu-id="28c5f-109">Element</span><span class="sxs-lookup"><span data-stu-id="28c5f-109">Member</span></span>|<span data-ttu-id="28c5f-110">Wert</span><span class="sxs-lookup"><span data-stu-id="28c5f-110">Value</span></span>|<span data-ttu-id="28c5f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28c5f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28c5f-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="28c5f-112">userDefined</span></span>|<span data-ttu-id="28c5f-113">0</span><span class="sxs-lookup"><span data-stu-id="28c5f-113">0</span></span>|<span data-ttu-id="28c5f-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="28c5f-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="28c5f-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="28c5f-115">asMessagesArrive</span></span>|<span data-ttu-id="28c5f-116">1</span><span class="sxs-lookup"><span data-stu-id="28c5f-116">1</span></span>|<span data-ttu-id="28c5f-117">Synchronisieren Sie wie Nachrichten eingehen.</span><span class="sxs-lookup"><span data-stu-id="28c5f-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="28c5f-118">Manuell</span><span class="sxs-lookup"><span data-stu-id="28c5f-118">manual</span></span>|<span data-ttu-id="28c5f-119">2</span><span class="sxs-lookup"><span data-stu-id="28c5f-119">2</span></span>|<span data-ttu-id="28c5f-120">Manuell synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="28c5f-120">Sync manually.</span></span>|
|<span data-ttu-id="28c5f-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="28c5f-121">fifteenMinutes</span></span>|<span data-ttu-id="28c5f-122">3</span><span class="sxs-lookup"><span data-stu-id="28c5f-122">3</span></span>|<span data-ttu-id="28c5f-123">Synchronisieren Sie alle 15 Minuten.</span><span class="sxs-lookup"><span data-stu-id="28c5f-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="28c5f-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="28c5f-124">thirtyMinutes</span></span>|<span data-ttu-id="28c5f-125">4</span><span class="sxs-lookup"><span data-stu-id="28c5f-125">4</span></span>|<span data-ttu-id="28c5f-126">Sync alle 30 Minuten.</span><span class="sxs-lookup"><span data-stu-id="28c5f-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="28c5f-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="28c5f-127">sixtyMinutes</span></span>|<span data-ttu-id="28c5f-128">5</span><span class="sxs-lookup"><span data-stu-id="28c5f-128">5</span></span>|<span data-ttu-id="28c5f-129">Sync alle 60 Minuten.</span><span class="sxs-lookup"><span data-stu-id="28c5f-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="28c5f-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="28c5f-130">basedOnMyUsage</span></span>|<span data-ttu-id="28c5f-131">6</span><span class="sxs-lookup"><span data-stu-id="28c5f-131">6</span></span>|<span data-ttu-id="28c5f-132">Die Synchronisierung basierend auf meine Verwendung.</span><span class="sxs-lookup"><span data-stu-id="28c5f-132">Sync based on my usage.</span></span>|





