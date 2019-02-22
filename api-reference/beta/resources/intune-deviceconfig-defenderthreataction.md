---
title: defenderThreatAction-Enumerationstyp
description: Die Standardaktion des Verteidigers für erkannte Schadsoftware.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4849f369aa5dd04a68599050aa097b2ac63f5ef1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154782"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="7043f-103">defenderThreatAction-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="7043f-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="7043f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7043f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7043f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7043f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7043f-106">Die Standardaktion des Verteidigers für erkannte Schadsoftware.</span><span class="sxs-lookup"><span data-stu-id="7043f-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="7043f-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="7043f-107">Members</span></span>
|<span data-ttu-id="7043f-108">Element</span><span class="sxs-lookup"><span data-stu-id="7043f-108">Member</span></span>|<span data-ttu-id="7043f-109">Wert</span><span class="sxs-lookup"><span data-stu-id="7043f-109">Value</span></span>|<span data-ttu-id="7043f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7043f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7043f-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="7043f-111">deviceDefault</span></span>|<span data-ttu-id="7043f-112">0</span><span class="sxs-lookup"><span data-stu-id="7043f-112">0</span></span>|<span data-ttu-id="7043f-113">Anwenden einer Aktion basierend auf der Updatedefinition.</span><span class="sxs-lookup"><span data-stu-id="7043f-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="7043f-114">clean</span><span class="sxs-lookup"><span data-stu-id="7043f-114">clean</span></span>|<span data-ttu-id="7043f-115">1</span><span class="sxs-lookup"><span data-stu-id="7043f-115">1</span></span>|<span data-ttu-id="7043f-116">BeReinigen Sie die erkannte Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="7043f-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="7043f-117">Quarantäne</span><span class="sxs-lookup"><span data-stu-id="7043f-117">quarantine</span></span>|<span data-ttu-id="7043f-118">2</span><span class="sxs-lookup"><span data-stu-id="7043f-118">2</span></span>|<span data-ttu-id="7043f-119">Isolieren Sie die erkannte Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="7043f-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="7043f-120">remove</span><span class="sxs-lookup"><span data-stu-id="7043f-120">remove</span></span>|<span data-ttu-id="7043f-121">3</span><span class="sxs-lookup"><span data-stu-id="7043f-121">3</span></span>|<span data-ttu-id="7043f-122">Entfernen Sie die erkannte Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="7043f-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="7043f-123">zulassen</span><span class="sxs-lookup"><span data-stu-id="7043f-123">allow</span></span>|<span data-ttu-id="7043f-124">4</span><span class="sxs-lookup"><span data-stu-id="7043f-124">4</span></span>|<span data-ttu-id="7043f-125">Die erkannte Bedrohung zulassen.</span><span class="sxs-lookup"><span data-stu-id="7043f-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="7043f-126">userDefined</span><span class="sxs-lookup"><span data-stu-id="7043f-126">userDefined</span></span>|<span data-ttu-id="7043f-127">5</span><span class="sxs-lookup"><span data-stu-id="7043f-127">5</span></span>|<span data-ttu-id="7043f-128">Der Benutzer kann die Aktion bestimmen, die mit der erkannten Bedrohung ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="7043f-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="7043f-129">Block</span><span class="sxs-lookup"><span data-stu-id="7043f-129">block</span></span>|<span data-ttu-id="7043f-130">6</span><span class="sxs-lookup"><span data-stu-id="7043f-130">6</span></span>|<span data-ttu-id="7043f-131">Die erkannte Bedrohung blockieren.</span><span class="sxs-lookup"><span data-stu-id="7043f-131">Block the detected threat.</span></span>|




