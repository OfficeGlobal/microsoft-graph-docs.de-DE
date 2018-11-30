---
title: DefenderThreatAction Enum-Typ
description: Defender Standardaktion durchführen erkannt Schadsoftware.
ms.openlocfilehash: a5eb108a3ab26596eec9abe838e3bbfe853d96d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018901"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="be17f-103">DefenderThreatAction Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="be17f-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="be17f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="be17f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be17f-105">Defender Standardaktion durchführen erkannt Schadsoftware.</span><span class="sxs-lookup"><span data-stu-id="be17f-105">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="be17f-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="be17f-106">Members</span></span>
|<span data-ttu-id="be17f-107">Element</span><span class="sxs-lookup"><span data-stu-id="be17f-107">Member</span></span>|<span data-ttu-id="be17f-108">Wert</span><span class="sxs-lookup"><span data-stu-id="be17f-108">Value</span></span>|<span data-ttu-id="be17f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be17f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be17f-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="be17f-110">deviceDefault</span></span>|<span data-ttu-id="be17f-111">0</span><span class="sxs-lookup"><span data-stu-id="be17f-111">0</span></span>|<span data-ttu-id="be17f-112">Wenden Sie Aktion basierend auf der Definition Update an.</span><span class="sxs-lookup"><span data-stu-id="be17f-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="be17f-113">clean</span><span class="sxs-lookup"><span data-stu-id="be17f-113">clean</span></span>|<span data-ttu-id="be17f-114">1</span><span class="sxs-lookup"><span data-stu-id="be17f-114">1</span></span>|<span data-ttu-id="be17f-115">Bereinigen der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="be17f-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="be17f-116">Quarantäne</span><span class="sxs-lookup"><span data-stu-id="be17f-116">quarantine</span></span>|<span data-ttu-id="be17f-117">2</span><span class="sxs-lookup"><span data-stu-id="be17f-117">2</span></span>|<span data-ttu-id="be17f-118">Isolieren Sie erkannte Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="be17f-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="be17f-119">remove</span><span class="sxs-lookup"><span data-stu-id="be17f-119">remove</span></span>|<span data-ttu-id="be17f-120">3</span><span class="sxs-lookup"><span data-stu-id="be17f-120">3</span></span>|<span data-ttu-id="be17f-121">Erkannte Bedrohung zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="be17f-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="be17f-122">zulassen</span><span class="sxs-lookup"><span data-stu-id="be17f-122">allow</span></span>|<span data-ttu-id="be17f-123">4</span><span class="sxs-lookup"><span data-stu-id="be17f-123">4</span></span>|<span data-ttu-id="be17f-124">Zulassen der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="be17f-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="be17f-125">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="be17f-125">userDefined</span></span>|<span data-ttu-id="be17f-126">5</span><span class="sxs-lookup"><span data-stu-id="be17f-126">5</span></span>|<span data-ttu-id="be17f-127">Ermöglicht es dem Benutzer die erkannten Bedrohung auszuführende Aktion zu bestimmen.</span><span class="sxs-lookup"><span data-stu-id="be17f-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="be17f-128">Blockieren</span><span class="sxs-lookup"><span data-stu-id="be17f-128">block</span></span>|<span data-ttu-id="be17f-129">6</span><span class="sxs-lookup"><span data-stu-id="be17f-129">6</span></span>|<span data-ttu-id="be17f-130">Blockieren der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="be17f-130">Block the detected threat.</span></span>|



