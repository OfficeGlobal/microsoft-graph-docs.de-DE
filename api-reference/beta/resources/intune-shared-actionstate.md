---
title: ActionState Enum-Typ
description: Status der Aktion auf dem Gerät
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 54f9a636cb579a234097f86aba8cf4e8fb8fefd0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421613"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="15cf0-103">ActionState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="15cf0-103">actionState enum type</span></span>

> <span data-ttu-id="15cf0-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="15cf0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15cf0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15cf0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15cf0-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15cf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15cf0-107">Status der Aktion auf dem Gerät</span><span class="sxs-lookup"><span data-stu-id="15cf0-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="15cf0-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="15cf0-108">Members</span></span>
|<span data-ttu-id="15cf0-109">Member</span><span class="sxs-lookup"><span data-stu-id="15cf0-109">Member</span></span>|<span data-ttu-id="15cf0-110">Wert</span><span class="sxs-lookup"><span data-stu-id="15cf0-110">Value</span></span>|<span data-ttu-id="15cf0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15cf0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15cf0-112">Keine</span><span class="sxs-lookup"><span data-stu-id="15cf0-112">none</span></span>|<span data-ttu-id="15cf0-113">0</span><span class="sxs-lookup"><span data-stu-id="15cf0-113">0</span></span>|<span data-ttu-id="15cf0-114">Nicht auf einen gültigen Action Zustand</span><span class="sxs-lookup"><span data-stu-id="15cf0-114">Not a valid action state</span></span>|
|<span data-ttu-id="15cf0-115">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="15cf0-115">pending</span></span>|<span data-ttu-id="15cf0-116">1</span><span class="sxs-lookup"><span data-stu-id="15cf0-116">1</span></span>|<span data-ttu-id="15cf0-117">Aktion steht noch aus</span><span class="sxs-lookup"><span data-stu-id="15cf0-117">Action is pending</span></span>|
|<span data-ttu-id="15cf0-118">abgebrochen</span><span class="sxs-lookup"><span data-stu-id="15cf0-118">canceled</span></span>|<span data-ttu-id="15cf0-119">2</span><span class="sxs-lookup"><span data-stu-id="15cf0-119">2</span></span>|<span data-ttu-id="15cf0-120">Aktion wurde abgebrochen.</span><span class="sxs-lookup"><span data-stu-id="15cf0-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="15cf0-121">aktive</span><span class="sxs-lookup"><span data-stu-id="15cf0-121">active</span></span>|<span data-ttu-id="15cf0-122">3</span><span class="sxs-lookup"><span data-stu-id="15cf0-122">3</span></span>|<span data-ttu-id="15cf0-123">Aktion ist aktiv.</span><span class="sxs-lookup"><span data-stu-id="15cf0-123">Action is active.</span></span>|
|<span data-ttu-id="15cf0-124">done</span><span class="sxs-lookup"><span data-stu-id="15cf0-124">done</span></span>|<span data-ttu-id="15cf0-125">4</span><span class="sxs-lookup"><span data-stu-id="15cf0-125">4</span></span>|<span data-ttu-id="15cf0-126">Aktion ohne Fehler abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="15cf0-126">Action completed without errors.</span></span>|
|<span data-ttu-id="15cf0-127">failed</span><span class="sxs-lookup"><span data-stu-id="15cf0-127">failed</span></span>|<span data-ttu-id="15cf0-128">5</span><span class="sxs-lookup"><span data-stu-id="15cf0-128">5</span></span>|<span data-ttu-id="15cf0-129">Aktion ist fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="15cf0-129">Action failed</span></span>|
|<span data-ttu-id="15cf0-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="15cf0-130">notSupported</span></span>|<span data-ttu-id="15cf0-131">6</span><span class="sxs-lookup"><span data-stu-id="15cf0-131">6</span></span>|<span data-ttu-id="15cf0-132">Aktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15cf0-132">Action is not supported.</span></span>|




