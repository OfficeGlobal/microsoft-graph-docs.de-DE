---
title: ActionState Enum-Typ
description: Status der Aktion auf dem Gerät
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 14ec93848deccb7d6bb21331095f9ecf4a881815
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990852"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="63219-103">ActionState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="63219-103">actionState enum type</span></span>

> <span data-ttu-id="63219-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="63219-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63219-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="63219-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63219-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="63219-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63219-107">Status der Aktion auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="63219-107">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="63219-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="63219-108">Members</span></span>
|<span data-ttu-id="63219-109">Element</span><span class="sxs-lookup"><span data-stu-id="63219-109">Member</span></span>|<span data-ttu-id="63219-110">Wert</span><span class="sxs-lookup"><span data-stu-id="63219-110">Value</span></span>|<span data-ttu-id="63219-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="63219-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63219-112">n/v</span><span class="sxs-lookup"><span data-stu-id="63219-112">none</span></span>|<span data-ttu-id="63219-113">0</span><span class="sxs-lookup"><span data-stu-id="63219-113">0</span></span>|<span data-ttu-id="63219-114">Nicht auf einen gültigen Action Zustand</span><span class="sxs-lookup"><span data-stu-id="63219-114">Not a valid action state</span></span>|
|<span data-ttu-id="63219-115">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="63219-115">pending</span></span>|<span data-ttu-id="63219-116">1</span><span class="sxs-lookup"><span data-stu-id="63219-116">1</span></span>|<span data-ttu-id="63219-117">Aktion steht noch aus</span><span class="sxs-lookup"><span data-stu-id="63219-117">Action is pending</span></span>|
|<span data-ttu-id="63219-118">abgebrochen</span><span class="sxs-lookup"><span data-stu-id="63219-118">canceled</span></span>|<span data-ttu-id="63219-119">2</span><span class="sxs-lookup"><span data-stu-id="63219-119">2</span></span>|<span data-ttu-id="63219-120">Aktion wurde abgebrochen.</span><span class="sxs-lookup"><span data-stu-id="63219-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="63219-121">aktive</span><span class="sxs-lookup"><span data-stu-id="63219-121">active</span></span>|<span data-ttu-id="63219-122">3</span><span class="sxs-lookup"><span data-stu-id="63219-122">3</span></span>|<span data-ttu-id="63219-123">Aktion ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="63219-123">Action is active.</span></span>|
|<span data-ttu-id="63219-124">done</span><span class="sxs-lookup"><span data-stu-id="63219-124">done</span></span>|<span data-ttu-id="63219-125">4</span><span class="sxs-lookup"><span data-stu-id="63219-125">4</span></span>|<span data-ttu-id="63219-126">Aktion ohne Fehler abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="63219-126">Action completed without errors.</span></span>|
|<span data-ttu-id="63219-127">failed</span><span class="sxs-lookup"><span data-stu-id="63219-127">failed</span></span>|<span data-ttu-id="63219-128">5</span><span class="sxs-lookup"><span data-stu-id="63219-128">5</span></span>|<span data-ttu-id="63219-129">Aktion ist fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="63219-129">Action failed</span></span>|
|<span data-ttu-id="63219-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="63219-130">notSupported</span></span>|<span data-ttu-id="63219-131">6</span><span class="sxs-lookup"><span data-stu-id="63219-131">6</span></span>|<span data-ttu-id="63219-132">Aktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="63219-132">Action is not supported.</span></span>|





