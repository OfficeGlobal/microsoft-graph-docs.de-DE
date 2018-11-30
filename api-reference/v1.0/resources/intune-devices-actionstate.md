---
title: ActionState Enum-Typ
description: Status der Aktion auf dem Gerät
ms.openlocfilehash: 1a18eb87cb4c9162777d16dc866de5f5766c87b1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019538"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="b9446-103">ActionState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="b9446-103">actionState enum type</span></span>

> <span data-ttu-id="b9446-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b9446-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9446-105">Status der Aktion auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="b9446-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="b9446-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="b9446-106">Members</span></span>
|<span data-ttu-id="b9446-107">Element</span><span class="sxs-lookup"><span data-stu-id="b9446-107">Member</span></span>|<span data-ttu-id="b9446-108">Wert</span><span class="sxs-lookup"><span data-stu-id="b9446-108">Value</span></span>|<span data-ttu-id="b9446-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9446-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9446-110">n/v</span><span class="sxs-lookup"><span data-stu-id="b9446-110">none</span></span>|<span data-ttu-id="b9446-111">0</span><span class="sxs-lookup"><span data-stu-id="b9446-111">0</span></span>|<span data-ttu-id="b9446-112">Nicht auf einen gültigen Action Zustand</span><span class="sxs-lookup"><span data-stu-id="b9446-112">Not a valid action state</span></span>|
|<span data-ttu-id="b9446-113">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="b9446-113">pending</span></span>|<span data-ttu-id="b9446-114">1</span><span class="sxs-lookup"><span data-stu-id="b9446-114">1</span></span>|<span data-ttu-id="b9446-115">Aktion steht noch aus</span><span class="sxs-lookup"><span data-stu-id="b9446-115">Action is pending</span></span>|
|<span data-ttu-id="b9446-116">abgebrochen</span><span class="sxs-lookup"><span data-stu-id="b9446-116">canceled</span></span>|<span data-ttu-id="b9446-117">2</span><span class="sxs-lookup"><span data-stu-id="b9446-117">2</span></span>|<span data-ttu-id="b9446-118">Aktion wurde abgebrochen.</span><span class="sxs-lookup"><span data-stu-id="b9446-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="b9446-119">aktive</span><span class="sxs-lookup"><span data-stu-id="b9446-119">active</span></span>|<span data-ttu-id="b9446-120">3</span><span class="sxs-lookup"><span data-stu-id="b9446-120">3</span></span>|<span data-ttu-id="b9446-121">Aktion ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="b9446-121">Action is active.</span></span>|
|<span data-ttu-id="b9446-122">done</span><span class="sxs-lookup"><span data-stu-id="b9446-122">done</span></span>|<span data-ttu-id="b9446-123">4</span><span class="sxs-lookup"><span data-stu-id="b9446-123">4</span></span>|<span data-ttu-id="b9446-124">Aktion ohne Fehler abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="b9446-124">Action completed without errors.</span></span>|
|<span data-ttu-id="b9446-125">failed</span><span class="sxs-lookup"><span data-stu-id="b9446-125">failed</span></span>|<span data-ttu-id="b9446-126">5</span><span class="sxs-lookup"><span data-stu-id="b9446-126">5</span></span>|<span data-ttu-id="b9446-127">Aktion ist fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="b9446-127">Action failed</span></span>|
|<span data-ttu-id="b9446-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="b9446-128">notSupported</span></span>|<span data-ttu-id="b9446-129">6</span><span class="sxs-lookup"><span data-stu-id="b9446-129">6</span></span>|<span data-ttu-id="b9446-130">Aktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9446-130">Action is not supported.</span></span>|



