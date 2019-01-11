---
title: DefenderThreatAction Enum-Typ
description: Defender Standardaktion durchführen erkannt Schadsoftware.
localization_priority: Normal
ms.openlocfilehash: ed84a16dbac493a3e962e37ba246d8d418782a91
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852822"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="5e795-103">DefenderThreatAction Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="5e795-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="5e795-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5e795-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e795-105">Defender Standardaktion durchführen erkannt Schadsoftware.</span><span class="sxs-lookup"><span data-stu-id="5e795-105">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="5e795-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="5e795-106">Members</span></span>
|<span data-ttu-id="5e795-107">Element</span><span class="sxs-lookup"><span data-stu-id="5e795-107">Member</span></span>|<span data-ttu-id="5e795-108">Wert</span><span class="sxs-lookup"><span data-stu-id="5e795-108">Value</span></span>|<span data-ttu-id="5e795-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5e795-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e795-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="5e795-110">deviceDefault</span></span>|<span data-ttu-id="5e795-111">0</span><span class="sxs-lookup"><span data-stu-id="5e795-111">0</span></span>|<span data-ttu-id="5e795-112">Wenden Sie Aktion basierend auf der Definition Update an.</span><span class="sxs-lookup"><span data-stu-id="5e795-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="5e795-113">clean</span><span class="sxs-lookup"><span data-stu-id="5e795-113">clean</span></span>|<span data-ttu-id="5e795-114">1</span><span class="sxs-lookup"><span data-stu-id="5e795-114">1</span></span>|<span data-ttu-id="5e795-115">Bereinigen der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="5e795-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="5e795-116">Quarantäne</span><span class="sxs-lookup"><span data-stu-id="5e795-116">quarantine</span></span>|<span data-ttu-id="5e795-117">2</span><span class="sxs-lookup"><span data-stu-id="5e795-117">2</span></span>|<span data-ttu-id="5e795-118">Isolieren Sie erkannte Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="5e795-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="5e795-119">remove</span><span class="sxs-lookup"><span data-stu-id="5e795-119">remove</span></span>|<span data-ttu-id="5e795-120">3</span><span class="sxs-lookup"><span data-stu-id="5e795-120">3</span></span>|<span data-ttu-id="5e795-121">Erkannte Bedrohung zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="5e795-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="5e795-122">zulassen</span><span class="sxs-lookup"><span data-stu-id="5e795-122">allow</span></span>|<span data-ttu-id="5e795-123">4</span><span class="sxs-lookup"><span data-stu-id="5e795-123">4</span></span>|<span data-ttu-id="5e795-124">Zulassen der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="5e795-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="5e795-125">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="5e795-125">userDefined</span></span>|<span data-ttu-id="5e795-126">5</span><span class="sxs-lookup"><span data-stu-id="5e795-126">5</span></span>|<span data-ttu-id="5e795-127">Ermöglicht es dem Benutzer die erkannten Bedrohung auszuführende Aktion zu bestimmen.</span><span class="sxs-lookup"><span data-stu-id="5e795-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="5e795-128">Blockieren</span><span class="sxs-lookup"><span data-stu-id="5e795-128">block</span></span>|<span data-ttu-id="5e795-129">6</span><span class="sxs-lookup"><span data-stu-id="5e795-129">6</span></span>|<span data-ttu-id="5e795-130">Blockieren der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="5e795-130">Block the detected threat.</span></span>|



