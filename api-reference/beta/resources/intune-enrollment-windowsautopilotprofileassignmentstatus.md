---
title: WindowsAutopilotProfileAssignmentStatus Enum-Typ
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 255aab9770305baa29e73278b3bfceec1079351a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321000"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="5d1fa-103">WindowsAutopilotProfileAssignmentStatus Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="5d1fa-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="5d1fa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5d1fa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d1fa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5d1fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d1fa-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5d1fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d1fa-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5d1fa-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="5d1fa-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="5d1fa-108">Members</span></span>
|<span data-ttu-id="5d1fa-109">Member</span><span class="sxs-lookup"><span data-stu-id="5d1fa-109">Member</span></span>|<span data-ttu-id="5d1fa-110">Wert</span><span class="sxs-lookup"><span data-stu-id="5d1fa-110">Value</span></span>|<span data-ttu-id="5d1fa-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d1fa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d1fa-112">unknown</span><span class="sxs-lookup"><span data-stu-id="5d1fa-112">unknown</span></span>|<span data-ttu-id="5d1fa-113">0</span><span class="sxs-lookup"><span data-stu-id="5d1fa-113">0</span></span>|<span data-ttu-id="5d1fa-114">Unbekannte Zuordnungsstatus</span><span class="sxs-lookup"><span data-stu-id="5d1fa-114">Unknown assignment status</span></span>|
|<span data-ttu-id="5d1fa-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="5d1fa-115">assignedInSync</span></span>|<span data-ttu-id="5d1fa-116">1</span><span class="sxs-lookup"><span data-stu-id="5d1fa-116">1</span></span>|<span data-ttu-id="5d1fa-117">Zugewiesene erfolgreich in Intune und Synchronisierung mit Windows automatische Pilotprogramm</span><span class="sxs-lookup"><span data-stu-id="5d1fa-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="5d1fa-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="5d1fa-118">assignedOutOfSync</span></span>|<span data-ttu-id="5d1fa-119">2</span><span class="sxs-lookup"><span data-stu-id="5d1fa-119">2</span></span>|<span data-ttu-id="5d1fa-120">Zugewiesene erfolgreich in Intune und nicht synchron mit Windows automatische Pilotprogramm</span><span class="sxs-lookup"><span data-stu-id="5d1fa-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="5d1fa-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="5d1fa-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="5d1fa-122">3</span><span class="sxs-lookup"><span data-stu-id="5d1fa-122">3</span></span>|<span data-ttu-id="5d1fa-123">Zugeordnete erfolgreich in Intune und entweder synchron oder synchron mit Windows automatische Pilotprogramm</span><span class="sxs-lookup"><span data-stu-id="5d1fa-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="5d1fa-124">nicht zugewiesen</span><span class="sxs-lookup"><span data-stu-id="5d1fa-124">notAssigned</span></span>|<span data-ttu-id="5d1fa-125">4</span><span class="sxs-lookup"><span data-stu-id="5d1fa-125">4</span></span>|<span data-ttu-id="5d1fa-126">Nicht zugewiesen</span><span class="sxs-lookup"><span data-stu-id="5d1fa-126">Not assigned</span></span>|
|<span data-ttu-id="5d1fa-127">Ausstehende</span><span class="sxs-lookup"><span data-stu-id="5d1fa-127">pending</span></span>|<span data-ttu-id="5d1fa-128">5</span><span class="sxs-lookup"><span data-stu-id="5d1fa-128">5</span></span>|<span data-ttu-id="5d1fa-129">Ausstehende Zuordnung</span><span class="sxs-lookup"><span data-stu-id="5d1fa-129">Pending assignment</span></span>|
|<span data-ttu-id="5d1fa-130">failed</span><span class="sxs-lookup"><span data-stu-id="5d1fa-130">failed</span></span>|<span data-ttu-id="5d1fa-131">6</span><span class="sxs-lookup"><span data-stu-id="5d1fa-131">6</span></span>| <span data-ttu-id="5d1fa-132">Fehler bei Zuweisung</span><span class="sxs-lookup"><span data-stu-id="5d1fa-132">Assignment failed</span></span>|





