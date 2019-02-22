---
title: emailSyncSchedule-Enumerationstyp
description: Mögliche Werte für den Zeitplan für die e-Mail-Synchronisierung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad725c393b68805c2d6ac2470718fd68a7b0f16d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174846"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="e2dda-103">emailSyncSchedule-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="e2dda-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="e2dda-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e2dda-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2dda-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e2dda-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2dda-106">Mögliche Werte für den Zeitplan für die e-Mail-Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="e2dda-106">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="e2dda-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="e2dda-107">Members</span></span>
|<span data-ttu-id="e2dda-108">Element</span><span class="sxs-lookup"><span data-stu-id="e2dda-108">Member</span></span>|<span data-ttu-id="e2dda-109">Wert</span><span class="sxs-lookup"><span data-stu-id="e2dda-109">Value</span></span>|<span data-ttu-id="e2dda-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2dda-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2dda-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="e2dda-111">userDefined</span></span>|<span data-ttu-id="e2dda-112">0</span><span class="sxs-lookup"><span data-stu-id="e2dda-112">0</span></span>|<span data-ttu-id="e2dda-113">Benutzerdefiniert, Standardwert, keine Absicht.</span><span class="sxs-lookup"><span data-stu-id="e2dda-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e2dda-114">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="e2dda-114">asMessagesArrive</span></span>|<span data-ttu-id="e2dda-115">1</span><span class="sxs-lookup"><span data-stu-id="e2dda-115">1</span></span>|<span data-ttu-id="e2dda-116">Als Nachrichten eingehen.</span><span class="sxs-lookup"><span data-stu-id="e2dda-116">Sync as messages arrive.</span></span>|
|<span data-ttu-id="e2dda-117">Manuell</span><span class="sxs-lookup"><span data-stu-id="e2dda-117">manual</span></span>|<span data-ttu-id="e2dda-118">2</span><span class="sxs-lookup"><span data-stu-id="e2dda-118">2</span></span>|<span data-ttu-id="e2dda-119">Manuell synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="e2dda-119">Sync manually.</span></span>|
|<span data-ttu-id="e2dda-120">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="e2dda-120">fifteenMinutes</span></span>|<span data-ttu-id="e2dda-121">3</span><span class="sxs-lookup"><span data-stu-id="e2dda-121">3</span></span>|<span data-ttu-id="e2dda-122">Alle fünfzehn Minuten synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="e2dda-122">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="e2dda-123">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="e2dda-123">thirtyMinutes</span></span>|<span data-ttu-id="e2dda-124">4</span><span class="sxs-lookup"><span data-stu-id="e2dda-124">4</span></span>|<span data-ttu-id="e2dda-125">Alle dreißig Minuten synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="e2dda-125">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="e2dda-126">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="e2dda-126">sixtyMinutes</span></span>|<span data-ttu-id="e2dda-127">5</span><span class="sxs-lookup"><span data-stu-id="e2dda-127">5</span></span>|<span data-ttu-id="e2dda-128">Alle 60 Minuten synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="e2dda-128">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="e2dda-129">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="e2dda-129">basedOnMyUsage</span></span>|<span data-ttu-id="e2dda-130">6</span><span class="sxs-lookup"><span data-stu-id="e2dda-130">6</span></span>|<span data-ttu-id="e2dda-131">Synchronisierung basierend auf meiner Verwendung.</span><span class="sxs-lookup"><span data-stu-id="e2dda-131">Sync based on my usage.</span></span>|




