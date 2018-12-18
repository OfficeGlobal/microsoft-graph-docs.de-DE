---
title: ResultantAppState Enum-Typ
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 7b45353867abe77143fb97755aff457e0c81deb8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319425"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="9b26c-103">ResultantAppState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="9b26c-103">resultantAppState enum type</span></span>

> <span data-ttu-id="9b26c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9b26c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b26c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9b26c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b26c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9b26c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b26c-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9b26c-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="9b26c-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="9b26c-108">Members</span></span>
|<span data-ttu-id="9b26c-109">Member</span><span class="sxs-lookup"><span data-stu-id="9b26c-109">Member</span></span>|<span data-ttu-id="9b26c-110">Wert</span><span class="sxs-lookup"><span data-stu-id="9b26c-110">Value</span></span>|<span data-ttu-id="9b26c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9b26c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b26c-112">installiert</span><span class="sxs-lookup"><span data-stu-id="9b26c-112">installed</span></span>|<span data-ttu-id="9b26c-113">1</span><span class="sxs-lookup"><span data-stu-id="9b26c-113">1</span></span>|<span data-ttu-id="9b26c-114">Die Anwendung wird ohne Fehler installiert.</span><span class="sxs-lookup"><span data-stu-id="9b26c-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="9b26c-115">failed</span><span class="sxs-lookup"><span data-stu-id="9b26c-115">failed</span></span>|<span data-ttu-id="9b26c-116">2</span><span class="sxs-lookup"><span data-stu-id="9b26c-116">2</span></span>|<span data-ttu-id="9b26c-117">Die Anwendung konnte nicht installiert werden.</span><span class="sxs-lookup"><span data-stu-id="9b26c-117">The application failed to install.</span></span>|
|<span data-ttu-id="9b26c-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="9b26c-118">notInstalled</span></span>|<span data-ttu-id="9b26c-119">3</span><span class="sxs-lookup"><span data-stu-id="9b26c-119">3</span></span>|<span data-ttu-id="9b26c-120">Die Anwendung ist nicht installiert.</span><span class="sxs-lookup"><span data-stu-id="9b26c-120">The application is not installed.</span></span>|
|<span data-ttu-id="9b26c-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="9b26c-121">uninstallFailed</span></span>|<span data-ttu-id="9b26c-122">4</span><span class="sxs-lookup"><span data-stu-id="9b26c-122">4</span></span>|<span data-ttu-id="9b26c-123">Die Anwendung konnte nicht deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="9b26c-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="9b26c-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="9b26c-124">pendingInstall</span></span>|<span data-ttu-id="9b26c-125">5</span><span class="sxs-lookup"><span data-stu-id="9b26c-125">5</span></span>|<span data-ttu-id="9b26c-126">Die Installation der Anwendung wird gerade durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="9b26c-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="9b26c-127">unknown</span><span class="sxs-lookup"><span data-stu-id="9b26c-127">unknown</span></span>|<span data-ttu-id="9b26c-128">99</span><span class="sxs-lookup"><span data-stu-id="9b26c-128">99</span></span>|<span data-ttu-id="9b26c-129">Der Status der Anwendung ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="9b26c-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="9b26c-130">notApplicable</span><span class="sxs-lookup"><span data-stu-id="9b26c-130">notApplicable</span></span>|<span data-ttu-id="9b26c-131">-1</span><span class="sxs-lookup"><span data-stu-id="9b26c-131">-1</span></span>|<span data-ttu-id="9b26c-132">Die Anwendung ist nicht anwendbar.</span><span class="sxs-lookup"><span data-stu-id="9b26c-132">The application is not applicable.</span></span>|





