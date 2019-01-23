---
title: DefenderThreatAction Enum-Typ
description: Defender Standardaktion durchführen erkannt Schadsoftware.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d092d5a23fc006a9accdf9062a27cd79f323d208
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400270"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="ee273-103">DefenderThreatAction Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="ee273-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="ee273-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ee273-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ee273-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ee273-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee273-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ee273-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee273-107">Defender Standardaktion durchführen erkannt Schadsoftware.</span><span class="sxs-lookup"><span data-stu-id="ee273-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="ee273-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="ee273-108">Members</span></span>
|<span data-ttu-id="ee273-109">Member</span><span class="sxs-lookup"><span data-stu-id="ee273-109">Member</span></span>|<span data-ttu-id="ee273-110">Wert</span><span class="sxs-lookup"><span data-stu-id="ee273-110">Value</span></span>|<span data-ttu-id="ee273-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee273-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee273-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ee273-112">deviceDefault</span></span>|<span data-ttu-id="ee273-113">0</span><span class="sxs-lookup"><span data-stu-id="ee273-113">0</span></span>|<span data-ttu-id="ee273-114">Wenden Sie Aktion basierend auf der Definition Update an.</span><span class="sxs-lookup"><span data-stu-id="ee273-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="ee273-115">clean</span><span class="sxs-lookup"><span data-stu-id="ee273-115">clean</span></span>|<span data-ttu-id="ee273-116">1</span><span class="sxs-lookup"><span data-stu-id="ee273-116">1</span></span>|<span data-ttu-id="ee273-117">Bereinigen der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="ee273-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="ee273-118">Quarantäne</span><span class="sxs-lookup"><span data-stu-id="ee273-118">quarantine</span></span>|<span data-ttu-id="ee273-119">2</span><span class="sxs-lookup"><span data-stu-id="ee273-119">2</span></span>|<span data-ttu-id="ee273-120">Isolieren Sie erkannte Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="ee273-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="ee273-121">remove</span><span class="sxs-lookup"><span data-stu-id="ee273-121">remove</span></span>|<span data-ttu-id="ee273-122">3</span><span class="sxs-lookup"><span data-stu-id="ee273-122">3</span></span>|<span data-ttu-id="ee273-123">Erkannte Bedrohung zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="ee273-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="ee273-124">zulassen</span><span class="sxs-lookup"><span data-stu-id="ee273-124">allow</span></span>|<span data-ttu-id="ee273-125">4</span><span class="sxs-lookup"><span data-stu-id="ee273-125">4</span></span>|<span data-ttu-id="ee273-126">Zulassen der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="ee273-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="ee273-127">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="ee273-127">userDefined</span></span>|<span data-ttu-id="ee273-128">5</span><span class="sxs-lookup"><span data-stu-id="ee273-128">5</span></span>|<span data-ttu-id="ee273-129">Ermöglicht es dem Benutzer die erkannten Bedrohung auszuführende Aktion zu bestimmen.</span><span class="sxs-lookup"><span data-stu-id="ee273-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="ee273-130">Blockieren</span><span class="sxs-lookup"><span data-stu-id="ee273-130">block</span></span>|<span data-ttu-id="ee273-131">6</span><span class="sxs-lookup"><span data-stu-id="ee273-131">6</span></span>|<span data-ttu-id="ee273-132">Blockieren der erkannten Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="ee273-132">Block the detected threat.</span></span>|




