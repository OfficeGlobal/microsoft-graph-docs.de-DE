---
title: ActionState Enum-Typ
description: Status der Aktion auf dem Gerät
author: tfitzmac
ms.openlocfilehash: 1f36c3a6709ade5860ff24cc8d10c2cb0294a471
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315106"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="e3bb3-103">ActionState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="e3bb3-103">actionState enum type</span></span>

> <span data-ttu-id="e3bb3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e3bb3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3bb3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3bb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3bb3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e3bb3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3bb3-107">Status der Aktion auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="e3bb3-107">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="e3bb3-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="e3bb3-108">Members</span></span>
|<span data-ttu-id="e3bb3-109">Member</span><span class="sxs-lookup"><span data-stu-id="e3bb3-109">Member</span></span>|<span data-ttu-id="e3bb3-110">Wert</span><span class="sxs-lookup"><span data-stu-id="e3bb3-110">Value</span></span>|<span data-ttu-id="e3bb3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3bb3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3bb3-112">Keine</span><span class="sxs-lookup"><span data-stu-id="e3bb3-112">none</span></span>|<span data-ttu-id="e3bb3-113">0</span><span class="sxs-lookup"><span data-stu-id="e3bb3-113">0</span></span>|<span data-ttu-id="e3bb3-114">Nicht auf einen gültigen Action Zustand</span><span class="sxs-lookup"><span data-stu-id="e3bb3-114">Not a valid action state</span></span>|
|<span data-ttu-id="e3bb3-115">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="e3bb3-115">pending</span></span>|<span data-ttu-id="e3bb3-116">1</span><span class="sxs-lookup"><span data-stu-id="e3bb3-116">1</span></span>|<span data-ttu-id="e3bb3-117">Aktion steht noch aus</span><span class="sxs-lookup"><span data-stu-id="e3bb3-117">Action is pending</span></span>|
|<span data-ttu-id="e3bb3-118">abgebrochen</span><span class="sxs-lookup"><span data-stu-id="e3bb3-118">canceled</span></span>|<span data-ttu-id="e3bb3-119">2</span><span class="sxs-lookup"><span data-stu-id="e3bb3-119">2</span></span>|<span data-ttu-id="e3bb3-120">Aktion wurde abgebrochen.</span><span class="sxs-lookup"><span data-stu-id="e3bb3-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="e3bb3-121">aktive</span><span class="sxs-lookup"><span data-stu-id="e3bb3-121">active</span></span>|<span data-ttu-id="e3bb3-122">3</span><span class="sxs-lookup"><span data-stu-id="e3bb3-122">3</span></span>|<span data-ttu-id="e3bb3-123">Aktion ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="e3bb3-123">Action is active.</span></span>|
|<span data-ttu-id="e3bb3-124">done</span><span class="sxs-lookup"><span data-stu-id="e3bb3-124">done</span></span>|<span data-ttu-id="e3bb3-125">4</span><span class="sxs-lookup"><span data-stu-id="e3bb3-125">4</span></span>|<span data-ttu-id="e3bb3-126">Aktion ohne Fehler abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="e3bb3-126">Action completed without errors.</span></span>|
|<span data-ttu-id="e3bb3-127">failed</span><span class="sxs-lookup"><span data-stu-id="e3bb3-127">failed</span></span>|<span data-ttu-id="e3bb3-128">5</span><span class="sxs-lookup"><span data-stu-id="e3bb3-128">5</span></span>|<span data-ttu-id="e3bb3-129">Aktion ist fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="e3bb3-129">Action failed</span></span>|
|<span data-ttu-id="e3bb3-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="e3bb3-130">notSupported</span></span>|<span data-ttu-id="e3bb3-131">6</span><span class="sxs-lookup"><span data-stu-id="e3bb3-131">6</span></span>|<span data-ttu-id="e3bb3-132">Aktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3bb3-132">Action is not supported.</span></span>|





