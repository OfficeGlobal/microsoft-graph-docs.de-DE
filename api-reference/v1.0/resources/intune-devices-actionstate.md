---
title: ActionState Enum-Typ
description: Status der Aktion auf dem Gerät
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c0c05e283b94473a5c8c43498ff5bf1dd82da7a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871939"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="055aa-103">ActionState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="055aa-103">actionState enum type</span></span>

> <span data-ttu-id="055aa-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="055aa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="055aa-105">Status der Aktion auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="055aa-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="055aa-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="055aa-106">Members</span></span>
|<span data-ttu-id="055aa-107">Element</span><span class="sxs-lookup"><span data-stu-id="055aa-107">Member</span></span>|<span data-ttu-id="055aa-108">Wert</span><span class="sxs-lookup"><span data-stu-id="055aa-108">Value</span></span>|<span data-ttu-id="055aa-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="055aa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="055aa-110">n/v</span><span class="sxs-lookup"><span data-stu-id="055aa-110">none</span></span>|<span data-ttu-id="055aa-111">0</span><span class="sxs-lookup"><span data-stu-id="055aa-111">0</span></span>|<span data-ttu-id="055aa-112">Nicht auf einen gültigen Action Zustand</span><span class="sxs-lookup"><span data-stu-id="055aa-112">Not a valid action state</span></span>|
|<span data-ttu-id="055aa-113">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="055aa-113">pending</span></span>|<span data-ttu-id="055aa-114">1</span><span class="sxs-lookup"><span data-stu-id="055aa-114">1</span></span>|<span data-ttu-id="055aa-115">Aktion steht noch aus</span><span class="sxs-lookup"><span data-stu-id="055aa-115">Action is pending</span></span>|
|<span data-ttu-id="055aa-116">abgebrochen</span><span class="sxs-lookup"><span data-stu-id="055aa-116">canceled</span></span>|<span data-ttu-id="055aa-117">2</span><span class="sxs-lookup"><span data-stu-id="055aa-117">2</span></span>|<span data-ttu-id="055aa-118">Aktion wurde abgebrochen.</span><span class="sxs-lookup"><span data-stu-id="055aa-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="055aa-119">aktive</span><span class="sxs-lookup"><span data-stu-id="055aa-119">active</span></span>|<span data-ttu-id="055aa-120">3</span><span class="sxs-lookup"><span data-stu-id="055aa-120">3</span></span>|<span data-ttu-id="055aa-121">Aktion ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="055aa-121">Action is active.</span></span>|
|<span data-ttu-id="055aa-122">done</span><span class="sxs-lookup"><span data-stu-id="055aa-122">done</span></span>|<span data-ttu-id="055aa-123">4</span><span class="sxs-lookup"><span data-stu-id="055aa-123">4</span></span>|<span data-ttu-id="055aa-124">Aktion ohne Fehler abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="055aa-124">Action completed without errors.</span></span>|
|<span data-ttu-id="055aa-125">failed</span><span class="sxs-lookup"><span data-stu-id="055aa-125">failed</span></span>|<span data-ttu-id="055aa-126">5</span><span class="sxs-lookup"><span data-stu-id="055aa-126">5</span></span>|<span data-ttu-id="055aa-127">Aktion ist fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="055aa-127">Action failed</span></span>|
|<span data-ttu-id="055aa-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="055aa-128">notSupported</span></span>|<span data-ttu-id="055aa-129">6</span><span class="sxs-lookup"><span data-stu-id="055aa-129">6</span></span>|<span data-ttu-id="055aa-130">Aktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="055aa-130">Action is not supported.</span></span>|



