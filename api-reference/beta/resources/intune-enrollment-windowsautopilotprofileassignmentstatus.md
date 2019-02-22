---
title: windowsAutopilotProfileAssignmentStatus-Enumerationstyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b5d1af0e6c91dced1aa12ae72c22430d16674c21
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156378"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="8bf56-103">windowsAutopilotProfileAssignmentStatus-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="8bf56-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="8bf56-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8bf56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bf56-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8bf56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bf56-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8bf56-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="8bf56-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="8bf56-107">Members</span></span>
|<span data-ttu-id="8bf56-108">Element</span><span class="sxs-lookup"><span data-stu-id="8bf56-108">Member</span></span>|<span data-ttu-id="8bf56-109">Wert</span><span class="sxs-lookup"><span data-stu-id="8bf56-109">Value</span></span>|<span data-ttu-id="8bf56-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8bf56-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bf56-111">unknown</span><span class="sxs-lookup"><span data-stu-id="8bf56-111">unknown</span></span>|<span data-ttu-id="8bf56-112">0</span><span class="sxs-lookup"><span data-stu-id="8bf56-112">0</span></span>|<span data-ttu-id="8bf56-113">UnBekannter Zuordnungsstatus</span><span class="sxs-lookup"><span data-stu-id="8bf56-113">Unknown assignment status</span></span>|
|<span data-ttu-id="8bf56-114">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="8bf56-114">assignedInSync</span></span>|<span data-ttu-id="8bf56-115">1</span><span class="sxs-lookup"><span data-stu-id="8bf56-115">1</span></span>|<span data-ttu-id="8bf56-116">Erfolgreich zugewiesen in InTune und synchron mit Windows Auto Pilot Program</span><span class="sxs-lookup"><span data-stu-id="8bf56-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="8bf56-117">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="8bf56-117">assignedOutOfSync</span></span>|<span data-ttu-id="8bf56-118">2</span><span class="sxs-lookup"><span data-stu-id="8bf56-118">2</span></span>|<span data-ttu-id="8bf56-119">Erfolgreich zugewiesen in InTune und nicht synchron mit Windows Auto Pilot Program</span><span class="sxs-lookup"><span data-stu-id="8bf56-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="8bf56-120">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="8bf56-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="8bf56-121">3</span><span class="sxs-lookup"><span data-stu-id="8bf56-121">3</span></span>|<span data-ttu-id="8bf56-122">Erfolgreich in InTune zugewiesen und entweder synchron oder nicht mit Windows Auto Pilot Program</span><span class="sxs-lookup"><span data-stu-id="8bf56-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="8bf56-123">notAssigned</span><span class="sxs-lookup"><span data-stu-id="8bf56-123">notAssigned</span></span>|<span data-ttu-id="8bf56-124">4</span><span class="sxs-lookup"><span data-stu-id="8bf56-124">4</span></span>|<span data-ttu-id="8bf56-125">Nicht zugewiesen</span><span class="sxs-lookup"><span data-stu-id="8bf56-125">Not assigned</span></span>|
|<span data-ttu-id="8bf56-126">ausstehenden</span><span class="sxs-lookup"><span data-stu-id="8bf56-126">pending</span></span>|<span data-ttu-id="8bf56-127">5</span><span class="sxs-lookup"><span data-stu-id="8bf56-127">5</span></span>|<span data-ttu-id="8bf56-128">AusStehende Zuweisung</span><span class="sxs-lookup"><span data-stu-id="8bf56-128">Pending assignment</span></span>|
|<span data-ttu-id="8bf56-129">failed</span><span class="sxs-lookup"><span data-stu-id="8bf56-129">failed</span></span>|<span data-ttu-id="8bf56-130">6</span><span class="sxs-lookup"><span data-stu-id="8bf56-130">6</span></span>| <span data-ttu-id="8bf56-131">Zuweisung fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="8bf56-131">Assignment failed</span></span>|




