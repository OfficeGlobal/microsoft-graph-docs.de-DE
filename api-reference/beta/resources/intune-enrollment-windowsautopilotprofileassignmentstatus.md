---
title: WindowsAutopilotProfileAssignmentStatus Enum-Typ
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 68612e2f4ccee46612c82237630efafda484b7e9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419121"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="69d3d-103">WindowsAutopilotProfileAssignmentStatus Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="69d3d-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="69d3d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="69d3d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="69d3d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="69d3d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69d3d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="69d3d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69d3d-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="69d3d-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="69d3d-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="69d3d-108">Members</span></span>
|<span data-ttu-id="69d3d-109">Member</span><span class="sxs-lookup"><span data-stu-id="69d3d-109">Member</span></span>|<span data-ttu-id="69d3d-110">Wert</span><span class="sxs-lookup"><span data-stu-id="69d3d-110">Value</span></span>|<span data-ttu-id="69d3d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69d3d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69d3d-112">unknown</span><span class="sxs-lookup"><span data-stu-id="69d3d-112">unknown</span></span>|<span data-ttu-id="69d3d-113">0</span><span class="sxs-lookup"><span data-stu-id="69d3d-113">0</span></span>|<span data-ttu-id="69d3d-114">Unbekannte Zuordnungsstatus</span><span class="sxs-lookup"><span data-stu-id="69d3d-114">Unknown assignment status</span></span>|
|<span data-ttu-id="69d3d-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="69d3d-115">assignedInSync</span></span>|<span data-ttu-id="69d3d-116">1</span><span class="sxs-lookup"><span data-stu-id="69d3d-116">1</span></span>|<span data-ttu-id="69d3d-117">Zugewiesene erfolgreich in Intune und Synchronisierung mit Windows automatische Pilotprogramm</span><span class="sxs-lookup"><span data-stu-id="69d3d-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="69d3d-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="69d3d-118">assignedOutOfSync</span></span>|<span data-ttu-id="69d3d-119">2</span><span class="sxs-lookup"><span data-stu-id="69d3d-119">2</span></span>|<span data-ttu-id="69d3d-120">Zugewiesene erfolgreich in Intune und nicht synchron mit Windows automatische Pilotprogramm</span><span class="sxs-lookup"><span data-stu-id="69d3d-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="69d3d-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="69d3d-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="69d3d-122">3</span><span class="sxs-lookup"><span data-stu-id="69d3d-122">3</span></span>|<span data-ttu-id="69d3d-123">Zugeordnete erfolgreich in Intune und entweder synchron oder synchron mit Windows automatische Pilotprogramm</span><span class="sxs-lookup"><span data-stu-id="69d3d-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="69d3d-124">nicht zugewiesen</span><span class="sxs-lookup"><span data-stu-id="69d3d-124">notAssigned</span></span>|<span data-ttu-id="69d3d-125">4</span><span class="sxs-lookup"><span data-stu-id="69d3d-125">4</span></span>|<span data-ttu-id="69d3d-126">Nicht zugewiesen</span><span class="sxs-lookup"><span data-stu-id="69d3d-126">Not assigned</span></span>|
|<span data-ttu-id="69d3d-127">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="69d3d-127">pending</span></span>|<span data-ttu-id="69d3d-128">5</span><span class="sxs-lookup"><span data-stu-id="69d3d-128">5</span></span>|<span data-ttu-id="69d3d-129">Ausstehende Zuordnung</span><span class="sxs-lookup"><span data-stu-id="69d3d-129">Pending assignment</span></span>|
|<span data-ttu-id="69d3d-130">failed</span><span class="sxs-lookup"><span data-stu-id="69d3d-130">failed</span></span>|<span data-ttu-id="69d3d-131">6</span><span class="sxs-lookup"><span data-stu-id="69d3d-131">6</span></span>| <span data-ttu-id="69d3d-132">Fehler bei Zuweisung</span><span class="sxs-lookup"><span data-stu-id="69d3d-132">Assignment failed</span></span>|




