---
title: ActionState Enum-Typ
description: Status der Aktion auf dem Gerät
author: tfitzmac
ms.openlocfilehash: 53ee72430ac646bf978a3167b87feaf398c8ac37
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333383"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="dc403-103">ActionState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="dc403-103">actionState enum type</span></span>

> <span data-ttu-id="dc403-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dc403-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc403-105">Status der Aktion auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="dc403-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="dc403-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="dc403-106">Members</span></span>
|<span data-ttu-id="dc403-107">Member</span><span class="sxs-lookup"><span data-stu-id="dc403-107">Member</span></span>|<span data-ttu-id="dc403-108">Wert</span><span class="sxs-lookup"><span data-stu-id="dc403-108">Value</span></span>|<span data-ttu-id="dc403-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dc403-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc403-110">Keine</span><span class="sxs-lookup"><span data-stu-id="dc403-110">none</span></span>|<span data-ttu-id="dc403-111">0</span><span class="sxs-lookup"><span data-stu-id="dc403-111">0</span></span>|<span data-ttu-id="dc403-112">Nicht auf einen gültigen Action Zustand</span><span class="sxs-lookup"><span data-stu-id="dc403-112">Not a valid action state</span></span>|
|<span data-ttu-id="dc403-113">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="dc403-113">pending</span></span>|<span data-ttu-id="dc403-114">1</span><span class="sxs-lookup"><span data-stu-id="dc403-114">1</span></span>|<span data-ttu-id="dc403-115">Aktion steht noch aus</span><span class="sxs-lookup"><span data-stu-id="dc403-115">Action is pending</span></span>|
|<span data-ttu-id="dc403-116">abgebrochen</span><span class="sxs-lookup"><span data-stu-id="dc403-116">canceled</span></span>|<span data-ttu-id="dc403-117">2</span><span class="sxs-lookup"><span data-stu-id="dc403-117">2</span></span>|<span data-ttu-id="dc403-118">Aktion wurde abgebrochen.</span><span class="sxs-lookup"><span data-stu-id="dc403-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="dc403-119">aktive</span><span class="sxs-lookup"><span data-stu-id="dc403-119">active</span></span>|<span data-ttu-id="dc403-120">3</span><span class="sxs-lookup"><span data-stu-id="dc403-120">3</span></span>|<span data-ttu-id="dc403-121">Aktion ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="dc403-121">Action is active.</span></span>|
|<span data-ttu-id="dc403-122">done</span><span class="sxs-lookup"><span data-stu-id="dc403-122">done</span></span>|<span data-ttu-id="dc403-123">4</span><span class="sxs-lookup"><span data-stu-id="dc403-123">4</span></span>|<span data-ttu-id="dc403-124">Aktion ohne Fehler abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="dc403-124">Action completed without errors.</span></span>|
|<span data-ttu-id="dc403-125">failed</span><span class="sxs-lookup"><span data-stu-id="dc403-125">failed</span></span>|<span data-ttu-id="dc403-126">5</span><span class="sxs-lookup"><span data-stu-id="dc403-126">5</span></span>|<span data-ttu-id="dc403-127">Aktion ist fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="dc403-127">Action failed</span></span>|
|<span data-ttu-id="dc403-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="dc403-128">notSupported</span></span>|<span data-ttu-id="dc403-129">6</span><span class="sxs-lookup"><span data-stu-id="dc403-129">6</span></span>|<span data-ttu-id="dc403-130">Aktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dc403-130">Action is not supported.</span></span>|



