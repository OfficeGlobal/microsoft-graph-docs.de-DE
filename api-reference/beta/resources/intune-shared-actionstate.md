---
title: ActionState Enum-Typ
description: Status der Aktion auf dem Gerät
ms.openlocfilehash: e0169bd690cdc8a26cc771948ebcf311f6fd6aa5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061388"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="522a4-103">ActionState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="522a4-103">actionState enum type</span></span>

> <span data-ttu-id="522a4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="522a4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="522a4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="522a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="522a4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="522a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="522a4-107">Status der Aktion auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="522a4-107">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="522a4-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="522a4-108">Members</span></span>
|<span data-ttu-id="522a4-109">Element</span><span class="sxs-lookup"><span data-stu-id="522a4-109">Member</span></span>|<span data-ttu-id="522a4-110">Wert</span><span class="sxs-lookup"><span data-stu-id="522a4-110">Value</span></span>|<span data-ttu-id="522a4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="522a4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="522a4-112">n/v</span><span class="sxs-lookup"><span data-stu-id="522a4-112">none</span></span>|<span data-ttu-id="522a4-113">0</span><span class="sxs-lookup"><span data-stu-id="522a4-113">0</span></span>|<span data-ttu-id="522a4-114">Nicht auf einen gültigen Action Zustand</span><span class="sxs-lookup"><span data-stu-id="522a4-114">Not a valid action state</span></span>|
|<span data-ttu-id="522a4-115">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="522a4-115">pending</span></span>|<span data-ttu-id="522a4-116">1</span><span class="sxs-lookup"><span data-stu-id="522a4-116">1</span></span>|<span data-ttu-id="522a4-117">Aktion steht noch aus</span><span class="sxs-lookup"><span data-stu-id="522a4-117">Action is pending</span></span>|
|<span data-ttu-id="522a4-118">abgebrochen</span><span class="sxs-lookup"><span data-stu-id="522a4-118">canceled</span></span>|<span data-ttu-id="522a4-119">2</span><span class="sxs-lookup"><span data-stu-id="522a4-119">2</span></span>|<span data-ttu-id="522a4-120">Aktion wurde abgebrochen.</span><span class="sxs-lookup"><span data-stu-id="522a4-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="522a4-121">aktive</span><span class="sxs-lookup"><span data-stu-id="522a4-121">active</span></span>|<span data-ttu-id="522a4-122">3</span><span class="sxs-lookup"><span data-stu-id="522a4-122">3</span></span>|<span data-ttu-id="522a4-123">Aktion ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="522a4-123">Action is active.</span></span>|
|<span data-ttu-id="522a4-124">done</span><span class="sxs-lookup"><span data-stu-id="522a4-124">done</span></span>|<span data-ttu-id="522a4-125">4</span><span class="sxs-lookup"><span data-stu-id="522a4-125">4</span></span>|<span data-ttu-id="522a4-126">Aktion ohne Fehler abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="522a4-126">Action completed without errors.</span></span>|
|<span data-ttu-id="522a4-127">failed</span><span class="sxs-lookup"><span data-stu-id="522a4-127">failed</span></span>|<span data-ttu-id="522a4-128">5</span><span class="sxs-lookup"><span data-stu-id="522a4-128">5</span></span>|<span data-ttu-id="522a4-129">Aktion ist fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="522a4-129">Action failed</span></span>|
|<span data-ttu-id="522a4-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="522a4-130">notSupported</span></span>|<span data-ttu-id="522a4-131">6</span><span class="sxs-lookup"><span data-stu-id="522a4-131">6</span></span>|<span data-ttu-id="522a4-132">Aktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="522a4-132">Action is not supported.</span></span>|





