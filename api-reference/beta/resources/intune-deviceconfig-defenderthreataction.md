---
title: DefenderThreatAction Enum-Typ
description: Defender Standardaktion durchführen erkannt Schadsoftware.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: fb54523f2817da328854e57a6672045e46ceb266
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938083"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="66c25-103">DefenderThreatAction Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="66c25-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="66c25-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="66c25-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66c25-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="66c25-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66c25-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="66c25-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66c25-107">Defender Standardaktion durchführen erkannt Schadsoftware.</span><span class="sxs-lookup"><span data-stu-id="66c25-107">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="66c25-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="66c25-108">Members</span></span>
|<span data-ttu-id="66c25-109">Element</span><span class="sxs-lookup"><span data-stu-id="66c25-109">Member</span></span>|<span data-ttu-id="66c25-110">Wert</span><span class="sxs-lookup"><span data-stu-id="66c25-110">Value</span></span>|<span data-ttu-id="66c25-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66c25-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66c25-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="66c25-112">deviceDefault</span></span>|<span data-ttu-id="66c25-113">0</span><span class="sxs-lookup"><span data-stu-id="66c25-113">0</span></span>|<span data-ttu-id="66c25-114">Wenden Sie Aktion basierend auf der Definition Update an.</span><span class="sxs-lookup"><span data-stu-id="66c25-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="66c25-115">clean</span><span class="sxs-lookup"><span data-stu-id="66c25-115">clean</span></span>|<span data-ttu-id="66c25-116">1</span><span class="sxs-lookup"><span data-stu-id="66c25-116">1</span></span>|<span data-ttu-id="66c25-117">Bereinigen der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="66c25-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="66c25-118">Quarantäne</span><span class="sxs-lookup"><span data-stu-id="66c25-118">quarantine</span></span>|<span data-ttu-id="66c25-119">2</span><span class="sxs-lookup"><span data-stu-id="66c25-119">2</span></span>|<span data-ttu-id="66c25-120">Isolieren Sie erkannte Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="66c25-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="66c25-121">remove</span><span class="sxs-lookup"><span data-stu-id="66c25-121">remove</span></span>|<span data-ttu-id="66c25-122">3</span><span class="sxs-lookup"><span data-stu-id="66c25-122">3</span></span>|<span data-ttu-id="66c25-123">Erkannte Bedrohung zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="66c25-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="66c25-124">zulassen</span><span class="sxs-lookup"><span data-stu-id="66c25-124">allow</span></span>|<span data-ttu-id="66c25-125">4</span><span class="sxs-lookup"><span data-stu-id="66c25-125">4</span></span>|<span data-ttu-id="66c25-126">Zulassen der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="66c25-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="66c25-127">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="66c25-127">userDefined</span></span>|<span data-ttu-id="66c25-128">5</span><span class="sxs-lookup"><span data-stu-id="66c25-128">5</span></span>|<span data-ttu-id="66c25-129">Ermöglicht es dem Benutzer die erkannten Bedrohung auszuführende Aktion zu bestimmen.</span><span class="sxs-lookup"><span data-stu-id="66c25-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="66c25-130">Blockieren</span><span class="sxs-lookup"><span data-stu-id="66c25-130">block</span></span>|<span data-ttu-id="66c25-131">6</span><span class="sxs-lookup"><span data-stu-id="66c25-131">6</span></span>|<span data-ttu-id="66c25-132">Blockieren der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="66c25-132">Block the detected threat.</span></span>|





