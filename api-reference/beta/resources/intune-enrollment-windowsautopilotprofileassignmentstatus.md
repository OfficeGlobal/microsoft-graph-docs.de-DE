---
title: WindowsAutopilotProfileAssignmentStatus Enum-Typ
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1427ffeb45862312d92fdf02a00a242725894d36
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962632"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="87df7-103">WindowsAutopilotProfileAssignmentStatus Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="87df7-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="87df7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="87df7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87df7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87df7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87df7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="87df7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87df7-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="87df7-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="87df7-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="87df7-108">Members</span></span>
|<span data-ttu-id="87df7-109">Element</span><span class="sxs-lookup"><span data-stu-id="87df7-109">Member</span></span>|<span data-ttu-id="87df7-110">Wert</span><span class="sxs-lookup"><span data-stu-id="87df7-110">Value</span></span>|<span data-ttu-id="87df7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87df7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87df7-112">unknown</span><span class="sxs-lookup"><span data-stu-id="87df7-112">unknown</span></span>|<span data-ttu-id="87df7-113">0</span><span class="sxs-lookup"><span data-stu-id="87df7-113">0</span></span>|<span data-ttu-id="87df7-114">Unbekannte Zuordnungsstatus</span><span class="sxs-lookup"><span data-stu-id="87df7-114">Unknown assignment status</span></span>|
|<span data-ttu-id="87df7-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="87df7-115">assignedInSync</span></span>|<span data-ttu-id="87df7-116">1</span><span class="sxs-lookup"><span data-stu-id="87df7-116">1</span></span>|<span data-ttu-id="87df7-117">Zugewiesene erfolgreich in Intune und Synchronisierung mit Windows automatische Pilotprogramm</span><span class="sxs-lookup"><span data-stu-id="87df7-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="87df7-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="87df7-118">assignedOutOfSync</span></span>|<span data-ttu-id="87df7-119">2</span><span class="sxs-lookup"><span data-stu-id="87df7-119">2</span></span>|<span data-ttu-id="87df7-120">Zugewiesene erfolgreich in Intune und nicht synchron mit Windows automatische Pilotprogramm</span><span class="sxs-lookup"><span data-stu-id="87df7-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="87df7-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="87df7-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="87df7-122">3</span><span class="sxs-lookup"><span data-stu-id="87df7-122">3</span></span>|<span data-ttu-id="87df7-123">Zugeordnete erfolgreich in Intune und entweder synchron oder synchron mit Windows automatische Pilotprogramm</span><span class="sxs-lookup"><span data-stu-id="87df7-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="87df7-124">nicht zugewiesen</span><span class="sxs-lookup"><span data-stu-id="87df7-124">notAssigned</span></span>|<span data-ttu-id="87df7-125">4</span><span class="sxs-lookup"><span data-stu-id="87df7-125">4</span></span>|<span data-ttu-id="87df7-126">Nicht zugewiesen</span><span class="sxs-lookup"><span data-stu-id="87df7-126">Not assigned</span></span>|
|<span data-ttu-id="87df7-127">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="87df7-127">pending</span></span>|<span data-ttu-id="87df7-128">5</span><span class="sxs-lookup"><span data-stu-id="87df7-128">5</span></span>|<span data-ttu-id="87df7-129">Ausstehende Zuordnung</span><span class="sxs-lookup"><span data-stu-id="87df7-129">Pending assignment</span></span>|
|<span data-ttu-id="87df7-130">failed</span><span class="sxs-lookup"><span data-stu-id="87df7-130">failed</span></span>|<span data-ttu-id="87df7-131">6</span><span class="sxs-lookup"><span data-stu-id="87df7-131">6</span></span>| <span data-ttu-id="87df7-132">Fehler bei Zuweisung</span><span class="sxs-lookup"><span data-stu-id="87df7-132">Assignment failed</span></span>|





