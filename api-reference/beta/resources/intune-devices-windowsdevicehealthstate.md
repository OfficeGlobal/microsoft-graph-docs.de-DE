---
title: WindowsDeviceHealthState Enum-Typ
description: Endpoint Protection-Computerstatus
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 628450b33a219e8408d5c5887c6902b78ae02bd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923943"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="240b6-103">WindowsDeviceHealthState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="240b6-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="240b6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="240b6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="240b6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="240b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="240b6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="240b6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="240b6-107">Endpoint Protection-Computerstatus</span><span class="sxs-lookup"><span data-stu-id="240b6-107">Computer endpoint protection state</span></span>
## <a name="members"></a><span data-ttu-id="240b6-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="240b6-108">Members</span></span>
|<span data-ttu-id="240b6-109">Element</span><span class="sxs-lookup"><span data-stu-id="240b6-109">Member</span></span>|<span data-ttu-id="240b6-110">Wert</span><span class="sxs-lookup"><span data-stu-id="240b6-110">Value</span></span>|<span data-ttu-id="240b6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="240b6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="240b6-112">clean</span><span class="sxs-lookup"><span data-stu-id="240b6-112">clean</span></span>|<span data-ttu-id="240b6-113">0</span><span class="sxs-lookup"><span data-stu-id="240b6-113">0</span></span>|<span data-ttu-id="240b6-114">Computer fehlerfrei ist und keine Aktion erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="240b6-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="240b6-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="240b6-115">fullScanPending</span></span>|<span data-ttu-id="240b6-116">1</span><span class="sxs-lookup"><span data-stu-id="240b6-116">1</span></span>|<span data-ttu-id="240b6-117">Computer befindet sich in ausstehen und vollständigen scan</span><span class="sxs-lookup"><span data-stu-id="240b6-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="240b6-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="240b6-118">rebootPending</span></span>|<span data-ttu-id="240b6-119">2</span><span class="sxs-lookup"><span data-stu-id="240b6-119">2</span></span>|<span data-ttu-id="240b6-120">Computer befindet sich in Ausstehender Neustart Zustand</span><span class="sxs-lookup"><span data-stu-id="240b6-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="240b6-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="240b6-121">manualStepsPending</span></span>|<span data-ttu-id="240b6-122">4</span><span class="sxs-lookup"><span data-stu-id="240b6-122">4</span></span>|<span data-ttu-id="240b6-123">Computer befindet sich in ausstehen und manuelle Schritte</span><span class="sxs-lookup"><span data-stu-id="240b6-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="240b6-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="240b6-124">offlineScanPending</span></span>|<span data-ttu-id="240b6-125">8</span><span class="sxs-lookup"><span data-stu-id="240b6-125">8</span></span>|<span data-ttu-id="240b6-126">Computer befindet sich in offline Scan ausstehen</span><span class="sxs-lookup"><span data-stu-id="240b6-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="240b6-127">critical</span><span class="sxs-lookup"><span data-stu-id="240b6-127">critical</span></span>|<span data-ttu-id="240b6-128">16</span><span class="sxs-lookup"><span data-stu-id="240b6-128">16</span></span>|<span data-ttu-id="240b6-129">Computer befindet sich im kritischen Fehlerzustand</span><span class="sxs-lookup"><span data-stu-id="240b6-129">Computer is in critical failure state</span></span>|





