---
title: defenderThreatAction-Enumerationstyp
description: Die Standardaktion des Verteidigers für erkannte Schadsoftware.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d3d48415e55ad246f75ca9b32bd169ee102fc67
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252315"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="135a3-103">defenderThreatAction-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="135a3-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="135a3-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="135a3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="135a3-105">Die Standardaktion des Verteidigers für erkannte Schadsoftware.</span><span class="sxs-lookup"><span data-stu-id="135a3-105">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="135a3-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="135a3-106">Members</span></span>
|<span data-ttu-id="135a3-107">Element</span><span class="sxs-lookup"><span data-stu-id="135a3-107">Member</span></span>|<span data-ttu-id="135a3-108">Wert</span><span class="sxs-lookup"><span data-stu-id="135a3-108">Value</span></span>|<span data-ttu-id="135a3-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="135a3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="135a3-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="135a3-110">deviceDefault</span></span>|<span data-ttu-id="135a3-111">0</span><span class="sxs-lookup"><span data-stu-id="135a3-111">0</span></span>|<span data-ttu-id="135a3-112">Anwenden einer Aktion basierend auf der Updatedefinition.</span><span class="sxs-lookup"><span data-stu-id="135a3-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="135a3-113">clean</span><span class="sxs-lookup"><span data-stu-id="135a3-113">clean</span></span>|<span data-ttu-id="135a3-114">1</span><span class="sxs-lookup"><span data-stu-id="135a3-114">1</span></span>|<span data-ttu-id="135a3-115">BeReinigen Sie die erkannte Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="135a3-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="135a3-116">Quarantäne</span><span class="sxs-lookup"><span data-stu-id="135a3-116">quarantine</span></span>|<span data-ttu-id="135a3-117">2</span><span class="sxs-lookup"><span data-stu-id="135a3-117">2</span></span>|<span data-ttu-id="135a3-118">Isolieren Sie die erkannte Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="135a3-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="135a3-119">remove</span><span class="sxs-lookup"><span data-stu-id="135a3-119">remove</span></span>|<span data-ttu-id="135a3-120">3</span><span class="sxs-lookup"><span data-stu-id="135a3-120">3</span></span>|<span data-ttu-id="135a3-121">Entfernen Sie die erkannte Bedrohung.</span><span class="sxs-lookup"><span data-stu-id="135a3-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="135a3-122">zulassen</span><span class="sxs-lookup"><span data-stu-id="135a3-122">allow</span></span>|<span data-ttu-id="135a3-123">4</span><span class="sxs-lookup"><span data-stu-id="135a3-123">4</span></span>|<span data-ttu-id="135a3-124">Die erkannte Bedrohung zulassen.</span><span class="sxs-lookup"><span data-stu-id="135a3-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="135a3-125">userDefined</span><span class="sxs-lookup"><span data-stu-id="135a3-125">userDefined</span></span>|<span data-ttu-id="135a3-126">5</span><span class="sxs-lookup"><span data-stu-id="135a3-126">5</span></span>|<span data-ttu-id="135a3-127">Der Benutzer kann die Aktion bestimmen, die mit der erkannten Bedrohung ausgeführt werden soll.</span><span class="sxs-lookup"><span data-stu-id="135a3-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="135a3-128">Block</span><span class="sxs-lookup"><span data-stu-id="135a3-128">block</span></span>|<span data-ttu-id="135a3-129">6</span><span class="sxs-lookup"><span data-stu-id="135a3-129">6</span></span>|<span data-ttu-id="135a3-130">Die erkannte Bedrohung blockieren.</span><span class="sxs-lookup"><span data-stu-id="135a3-130">Block the detected threat.</span></span>|



