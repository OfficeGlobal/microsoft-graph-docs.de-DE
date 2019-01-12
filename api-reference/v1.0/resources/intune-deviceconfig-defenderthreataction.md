---
title: DefenderThreatAction Enum-Typ
description: Defender Standardaktion durchführen erkannt Schadsoftware.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 51aa26483ac6b79d48567f7e5950733def31f01e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976646"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="9c896-103">DefenderThreatAction Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="9c896-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="9c896-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9c896-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c896-105">Defender Standardaktion durchführen erkannt Schadsoftware.</span><span class="sxs-lookup"><span data-stu-id="9c896-105">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="9c896-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="9c896-106">Members</span></span>
|<span data-ttu-id="9c896-107">Element</span><span class="sxs-lookup"><span data-stu-id="9c896-107">Member</span></span>|<span data-ttu-id="9c896-108">Wert</span><span class="sxs-lookup"><span data-stu-id="9c896-108">Value</span></span>|<span data-ttu-id="9c896-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c896-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c896-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9c896-110">deviceDefault</span></span>|<span data-ttu-id="9c896-111">0</span><span class="sxs-lookup"><span data-stu-id="9c896-111">0</span></span>|<span data-ttu-id="9c896-112">Wenden Sie Aktion basierend auf der Definition Update an.</span><span class="sxs-lookup"><span data-stu-id="9c896-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="9c896-113">clean</span><span class="sxs-lookup"><span data-stu-id="9c896-113">clean</span></span>|<span data-ttu-id="9c896-114">1</span><span class="sxs-lookup"><span data-stu-id="9c896-114">1</span></span>|<span data-ttu-id="9c896-115">Bereinigen der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="9c896-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="9c896-116">Quarantäne</span><span class="sxs-lookup"><span data-stu-id="9c896-116">quarantine</span></span>|<span data-ttu-id="9c896-117">2</span><span class="sxs-lookup"><span data-stu-id="9c896-117">2</span></span>|<span data-ttu-id="9c896-118">Isolieren Sie erkannte Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="9c896-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="9c896-119">remove</span><span class="sxs-lookup"><span data-stu-id="9c896-119">remove</span></span>|<span data-ttu-id="9c896-120">3</span><span class="sxs-lookup"><span data-stu-id="9c896-120">3</span></span>|<span data-ttu-id="9c896-121">Erkannte Bedrohung zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="9c896-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="9c896-122">zulassen</span><span class="sxs-lookup"><span data-stu-id="9c896-122">allow</span></span>|<span data-ttu-id="9c896-123">4</span><span class="sxs-lookup"><span data-stu-id="9c896-123">4</span></span>|<span data-ttu-id="9c896-124">Zulassen der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="9c896-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="9c896-125">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="9c896-125">userDefined</span></span>|<span data-ttu-id="9c896-126">5</span><span class="sxs-lookup"><span data-stu-id="9c896-126">5</span></span>|<span data-ttu-id="9c896-127">Ermöglicht es dem Benutzer die erkannten Bedrohung auszuführende Aktion zu bestimmen.</span><span class="sxs-lookup"><span data-stu-id="9c896-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="9c896-128">Blockieren</span><span class="sxs-lookup"><span data-stu-id="9c896-128">block</span></span>|<span data-ttu-id="9c896-129">6</span><span class="sxs-lookup"><span data-stu-id="9c896-129">6</span></span>|<span data-ttu-id="9c896-130">Blockieren der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="9c896-130">Block the detected threat.</span></span>|



