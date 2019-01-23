---
title: WindowsDeviceHealthState Enum-Typ
description: Endpoint Protection-Computerstatus
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2d971de9b20780bb51a19c3417384a0ca0563452
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416349"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="c63b1-103">WindowsDeviceHealthState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="c63b1-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="c63b1-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c63b1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c63b1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c63b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c63b1-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c63b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c63b1-107">Endpoint Protection-Computerstatus</span><span class="sxs-lookup"><span data-stu-id="c63b1-107">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="c63b1-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="c63b1-108">Members</span></span>
|<span data-ttu-id="c63b1-109">Member</span><span class="sxs-lookup"><span data-stu-id="c63b1-109">Member</span></span>|<span data-ttu-id="c63b1-110">Wert</span><span class="sxs-lookup"><span data-stu-id="c63b1-110">Value</span></span>|<span data-ttu-id="c63b1-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c63b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c63b1-112">clean</span><span class="sxs-lookup"><span data-stu-id="c63b1-112">clean</span></span>|<span data-ttu-id="c63b1-113">0</span><span class="sxs-lookup"><span data-stu-id="c63b1-113">0</span></span>|<span data-ttu-id="c63b1-114">Computer fehlerfrei ist und keine Aktion erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="c63b1-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="c63b1-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="c63b1-115">fullScanPending</span></span>|<span data-ttu-id="c63b1-116">1</span><span class="sxs-lookup"><span data-stu-id="c63b1-116">1</span></span>|<span data-ttu-id="c63b1-117">Computer befindet sich in ausstehen und vollständigen scan</span><span class="sxs-lookup"><span data-stu-id="c63b1-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="c63b1-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="c63b1-118">rebootPending</span></span>|<span data-ttu-id="c63b1-119">2</span><span class="sxs-lookup"><span data-stu-id="c63b1-119">2</span></span>|<span data-ttu-id="c63b1-120">Computer befindet sich in Ausstehender Neustart Zustand</span><span class="sxs-lookup"><span data-stu-id="c63b1-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="c63b1-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="c63b1-121">manualStepsPending</span></span>|<span data-ttu-id="c63b1-122">4</span><span class="sxs-lookup"><span data-stu-id="c63b1-122">4</span></span>|<span data-ttu-id="c63b1-123">Computer befindet sich in ausstehen und manuelle Schritte</span><span class="sxs-lookup"><span data-stu-id="c63b1-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="c63b1-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="c63b1-124">offlineScanPending</span></span>|<span data-ttu-id="c63b1-125">8</span><span class="sxs-lookup"><span data-stu-id="c63b1-125">8</span></span>|<span data-ttu-id="c63b1-126">Computer befindet sich in offline Scan ausstehen</span><span class="sxs-lookup"><span data-stu-id="c63b1-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="c63b1-127">critical</span><span class="sxs-lookup"><span data-stu-id="c63b1-127">critical</span></span>|<span data-ttu-id="c63b1-128">16</span><span class="sxs-lookup"><span data-stu-id="c63b1-128">16</span></span>|<span data-ttu-id="c63b1-129">Computer befindet sich im kritischen Fehlerzustand</span><span class="sxs-lookup"><span data-stu-id="c63b1-129">Computer is in critical failure state</span></span>|




