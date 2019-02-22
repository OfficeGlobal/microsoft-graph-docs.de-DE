---
title: windowsDeviceHealthState-Enumerationstyp
description: Schutzstatus des Computer Endpunkts
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb335cd39e6cbcd00f754faae8f7784001c424b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156168"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="a4115-103">windowsDeviceHealthState-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="a4115-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="a4115-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a4115-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4115-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a4115-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4115-106">Schutzstatus des Computer Endpunkts</span><span class="sxs-lookup"><span data-stu-id="a4115-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="a4115-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="a4115-107">Members</span></span>
|<span data-ttu-id="a4115-108">Element</span><span class="sxs-lookup"><span data-stu-id="a4115-108">Member</span></span>|<span data-ttu-id="a4115-109">Wert</span><span class="sxs-lookup"><span data-stu-id="a4115-109">Value</span></span>|<span data-ttu-id="a4115-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a4115-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4115-111">clean</span><span class="sxs-lookup"><span data-stu-id="a4115-111">clean</span></span>|<span data-ttu-id="a4115-112">0</span><span class="sxs-lookup"><span data-stu-id="a4115-112">0</span></span>|<span data-ttu-id="a4115-113">Der Computer ist sauber, und es ist keine Aktion erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a4115-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="a4115-114">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="a4115-114">fullScanPending</span></span>|<span data-ttu-id="a4115-115">1</span><span class="sxs-lookup"><span data-stu-id="a4115-115">1</span></span>|<span data-ttu-id="a4115-116">Der Computer ist in ausstehender vollständiger Scanstatus</span><span class="sxs-lookup"><span data-stu-id="a4115-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="a4115-117">rebootPending</span><span class="sxs-lookup"><span data-stu-id="a4115-117">rebootPending</span></span>|<span data-ttu-id="a4115-118">2</span><span class="sxs-lookup"><span data-stu-id="a4115-118">2</span></span>|<span data-ttu-id="a4115-119">Der Computer befindet sich im ausstehenden Neustartstatus</span><span class="sxs-lookup"><span data-stu-id="a4115-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="a4115-120">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="a4115-120">manualStepsPending</span></span>|<span data-ttu-id="a4115-121">4</span><span class="sxs-lookup"><span data-stu-id="a4115-121">4</span></span>|<span data-ttu-id="a4115-122">Der Computer befindet sich in ausstehenden manuellen Schritten Status</span><span class="sxs-lookup"><span data-stu-id="a4115-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="a4115-123">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="a4115-123">offlineScanPending</span></span>|<span data-ttu-id="a4115-124">8</span><span class="sxs-lookup"><span data-stu-id="a4115-124">8</span></span>|<span data-ttu-id="a4115-125">Der Computer befindet sich im ausstehenden Offline Scanstatus</span><span class="sxs-lookup"><span data-stu-id="a4115-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="a4115-126">critical</span><span class="sxs-lookup"><span data-stu-id="a4115-126">critical</span></span>|<span data-ttu-id="a4115-127">16</span><span class="sxs-lookup"><span data-stu-id="a4115-127">16</span></span>|<span data-ttu-id="a4115-128">Der Computer befindet sich im Status "kritisch"</span><span class="sxs-lookup"><span data-stu-id="a4115-128">Computer is in critical failure state</span></span>|




