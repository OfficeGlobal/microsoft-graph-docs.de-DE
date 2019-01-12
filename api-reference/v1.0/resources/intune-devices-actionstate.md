---
title: ActionState Enum-Typ
description: Status der Aktion auf dem Gerät
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5579d8de986a764cd96e42dff30c007449130b0b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922445"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="a8221-103">ActionState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="a8221-103">actionState enum type</span></span>

> <span data-ttu-id="a8221-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a8221-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8221-105">Status der Aktion auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="a8221-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="a8221-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="a8221-106">Members</span></span>
|<span data-ttu-id="a8221-107">Element</span><span class="sxs-lookup"><span data-stu-id="a8221-107">Member</span></span>|<span data-ttu-id="a8221-108">Wert</span><span class="sxs-lookup"><span data-stu-id="a8221-108">Value</span></span>|<span data-ttu-id="a8221-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8221-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8221-110">n/v</span><span class="sxs-lookup"><span data-stu-id="a8221-110">none</span></span>|<span data-ttu-id="a8221-111">0</span><span class="sxs-lookup"><span data-stu-id="a8221-111">0</span></span>|<span data-ttu-id="a8221-112">Nicht auf einen gültigen Action Zustand</span><span class="sxs-lookup"><span data-stu-id="a8221-112">Not a valid action state</span></span>|
|<span data-ttu-id="a8221-113">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="a8221-113">pending</span></span>|<span data-ttu-id="a8221-114">1</span><span class="sxs-lookup"><span data-stu-id="a8221-114">1</span></span>|<span data-ttu-id="a8221-115">Aktion steht noch aus</span><span class="sxs-lookup"><span data-stu-id="a8221-115">Action is pending</span></span>|
|<span data-ttu-id="a8221-116">abgebrochen</span><span class="sxs-lookup"><span data-stu-id="a8221-116">canceled</span></span>|<span data-ttu-id="a8221-117">2</span><span class="sxs-lookup"><span data-stu-id="a8221-117">2</span></span>|<span data-ttu-id="a8221-118">Aktion wurde abgebrochen.</span><span class="sxs-lookup"><span data-stu-id="a8221-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="a8221-119">aktive</span><span class="sxs-lookup"><span data-stu-id="a8221-119">active</span></span>|<span data-ttu-id="a8221-120">3</span><span class="sxs-lookup"><span data-stu-id="a8221-120">3</span></span>|<span data-ttu-id="a8221-121">Aktion ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="a8221-121">Action is active.</span></span>|
|<span data-ttu-id="a8221-122">done</span><span class="sxs-lookup"><span data-stu-id="a8221-122">done</span></span>|<span data-ttu-id="a8221-123">4</span><span class="sxs-lookup"><span data-stu-id="a8221-123">4</span></span>|<span data-ttu-id="a8221-124">Aktion ohne Fehler abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="a8221-124">Action completed without errors.</span></span>|
|<span data-ttu-id="a8221-125">failed</span><span class="sxs-lookup"><span data-stu-id="a8221-125">failed</span></span>|<span data-ttu-id="a8221-126">5</span><span class="sxs-lookup"><span data-stu-id="a8221-126">5</span></span>|<span data-ttu-id="a8221-127">Aktion ist fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="a8221-127">Action failed</span></span>|
|<span data-ttu-id="a8221-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="a8221-128">notSupported</span></span>|<span data-ttu-id="a8221-129">6</span><span class="sxs-lookup"><span data-stu-id="a8221-129">6</span></span>|<span data-ttu-id="a8221-130">Aktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8221-130">Action is not supported.</span></span>|



