---
title: ResultantAppState Enum-Typ
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b97f8f9fc44faf0c27c31f8bab60103547fcf743
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947288"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="e3688-103">ResultantAppState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="e3688-103">resultantAppState enum type</span></span>

> <span data-ttu-id="e3688-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e3688-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3688-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3688-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3688-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e3688-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3688-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e3688-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="e3688-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="e3688-108">Members</span></span>
|<span data-ttu-id="e3688-109">Element</span><span class="sxs-lookup"><span data-stu-id="e3688-109">Member</span></span>|<span data-ttu-id="e3688-110">Wert</span><span class="sxs-lookup"><span data-stu-id="e3688-110">Value</span></span>|<span data-ttu-id="e3688-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3688-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3688-112">installiert</span><span class="sxs-lookup"><span data-stu-id="e3688-112">installed</span></span>|<span data-ttu-id="e3688-113">1</span><span class="sxs-lookup"><span data-stu-id="e3688-113">1</span></span>|<span data-ttu-id="e3688-114">Die Anwendung wird ohne Fehler installiert.</span><span class="sxs-lookup"><span data-stu-id="e3688-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="e3688-115">failed</span><span class="sxs-lookup"><span data-stu-id="e3688-115">failed</span></span>|<span data-ttu-id="e3688-116">2</span><span class="sxs-lookup"><span data-stu-id="e3688-116">2</span></span>|<span data-ttu-id="e3688-117">Die Anwendung konnte nicht installiert werden.</span><span class="sxs-lookup"><span data-stu-id="e3688-117">The application failed to install.</span></span>|
|<span data-ttu-id="e3688-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="e3688-118">notInstalled</span></span>|<span data-ttu-id="e3688-119">3</span><span class="sxs-lookup"><span data-stu-id="e3688-119">3</span></span>|<span data-ttu-id="e3688-120">Die Anwendung ist nicht installiert.</span><span class="sxs-lookup"><span data-stu-id="e3688-120">The application is not installed.</span></span>|
|<span data-ttu-id="e3688-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="e3688-121">uninstallFailed</span></span>|<span data-ttu-id="e3688-122">4</span><span class="sxs-lookup"><span data-stu-id="e3688-122">4</span></span>|<span data-ttu-id="e3688-123">Die Anwendung konnte nicht deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="e3688-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="e3688-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="e3688-124">pendingInstall</span></span>|<span data-ttu-id="e3688-125">5</span><span class="sxs-lookup"><span data-stu-id="e3688-125">5</span></span>|<span data-ttu-id="e3688-126">Die Installation der Anwendung wird gerade durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="e3688-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="e3688-127">unknown</span><span class="sxs-lookup"><span data-stu-id="e3688-127">unknown</span></span>|<span data-ttu-id="e3688-128">99</span><span class="sxs-lookup"><span data-stu-id="e3688-128">99</span></span>|<span data-ttu-id="e3688-129">Der Status der Anwendung ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="e3688-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="e3688-130">notApplicable</span><span class="sxs-lookup"><span data-stu-id="e3688-130">notApplicable</span></span>|<span data-ttu-id="e3688-131">-1</span><span class="sxs-lookup"><span data-stu-id="e3688-131">-1</span></span>|<span data-ttu-id="e3688-132">Die Anwendung ist nicht anwendbar.</span><span class="sxs-lookup"><span data-stu-id="e3688-132">The application is not applicable.</span></span>|





