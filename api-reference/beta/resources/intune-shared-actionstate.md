---
title: ActionState Enum-Typ
description: Status der Aktion auf dem Gerät
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af8bb3869171faee5907b4a3f1921bcb70044aec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829904"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="fcde1-103">ActionState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="fcde1-103">actionState enum type</span></span>

> <span data-ttu-id="fcde1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fcde1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcde1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fcde1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fcde1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fcde1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcde1-107">Status der Aktion auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="fcde1-107">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="fcde1-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="fcde1-108">Members</span></span>
|<span data-ttu-id="fcde1-109">Element</span><span class="sxs-lookup"><span data-stu-id="fcde1-109">Member</span></span>|<span data-ttu-id="fcde1-110">Wert</span><span class="sxs-lookup"><span data-stu-id="fcde1-110">Value</span></span>|<span data-ttu-id="fcde1-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fcde1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcde1-112">n/v</span><span class="sxs-lookup"><span data-stu-id="fcde1-112">none</span></span>|<span data-ttu-id="fcde1-113">0</span><span class="sxs-lookup"><span data-stu-id="fcde1-113">0</span></span>|<span data-ttu-id="fcde1-114">Nicht auf einen gültigen Action Zustand</span><span class="sxs-lookup"><span data-stu-id="fcde1-114">Not a valid action state</span></span>|
|<span data-ttu-id="fcde1-115">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="fcde1-115">pending</span></span>|<span data-ttu-id="fcde1-116">1</span><span class="sxs-lookup"><span data-stu-id="fcde1-116">1</span></span>|<span data-ttu-id="fcde1-117">Aktion steht noch aus</span><span class="sxs-lookup"><span data-stu-id="fcde1-117">Action is pending</span></span>|
|<span data-ttu-id="fcde1-118">abgebrochen</span><span class="sxs-lookup"><span data-stu-id="fcde1-118">canceled</span></span>|<span data-ttu-id="fcde1-119">2</span><span class="sxs-lookup"><span data-stu-id="fcde1-119">2</span></span>|<span data-ttu-id="fcde1-120">Aktion wurde abgebrochen.</span><span class="sxs-lookup"><span data-stu-id="fcde1-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="fcde1-121">aktive</span><span class="sxs-lookup"><span data-stu-id="fcde1-121">active</span></span>|<span data-ttu-id="fcde1-122">3</span><span class="sxs-lookup"><span data-stu-id="fcde1-122">3</span></span>|<span data-ttu-id="fcde1-123">Aktion ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="fcde1-123">Action is active.</span></span>|
|<span data-ttu-id="fcde1-124">done</span><span class="sxs-lookup"><span data-stu-id="fcde1-124">done</span></span>|<span data-ttu-id="fcde1-125">4</span><span class="sxs-lookup"><span data-stu-id="fcde1-125">4</span></span>|<span data-ttu-id="fcde1-126">Aktion ohne Fehler abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="fcde1-126">Action completed without errors.</span></span>|
|<span data-ttu-id="fcde1-127">failed</span><span class="sxs-lookup"><span data-stu-id="fcde1-127">failed</span></span>|<span data-ttu-id="fcde1-128">5</span><span class="sxs-lookup"><span data-stu-id="fcde1-128">5</span></span>|<span data-ttu-id="fcde1-129">Aktion ist fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="fcde1-129">Action failed</span></span>|
|<span data-ttu-id="fcde1-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="fcde1-130">notSupported</span></span>|<span data-ttu-id="fcde1-131">6</span><span class="sxs-lookup"><span data-stu-id="fcde1-131">6</span></span>|<span data-ttu-id="fcde1-132">Aktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fcde1-132">Action is not supported.</span></span>|





