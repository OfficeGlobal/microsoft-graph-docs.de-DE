---
title: InstallState Enum-Typ
description: Mögliche Werte für Installationsstatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 92fa9887760835a02c26858fb11503a0841d912e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985382"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="1101e-103">InstallState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="1101e-103">installState enum type</span></span>

> <span data-ttu-id="1101e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1101e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1101e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1101e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1101e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1101e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1101e-107">Mögliche Werte für Installationsstatus.</span><span class="sxs-lookup"><span data-stu-id="1101e-107">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="1101e-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="1101e-108">Members</span></span>
|<span data-ttu-id="1101e-109">Element</span><span class="sxs-lookup"><span data-stu-id="1101e-109">Member</span></span>|<span data-ttu-id="1101e-110">Wert</span><span class="sxs-lookup"><span data-stu-id="1101e-110">Value</span></span>|<span data-ttu-id="1101e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1101e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1101e-112">notApplicable</span><span class="sxs-lookup"><span data-stu-id="1101e-112">notApplicable</span></span>|<span data-ttu-id="1101e-113">0</span><span class="sxs-lookup"><span data-stu-id="1101e-113">0</span></span>|<span data-ttu-id="1101e-114">Nicht zutreffend.</span><span class="sxs-lookup"><span data-stu-id="1101e-114">Not Applicable.</span></span>|
|<span data-ttu-id="1101e-115">installiert</span><span class="sxs-lookup"><span data-stu-id="1101e-115">installed</span></span>|<span data-ttu-id="1101e-116">1</span><span class="sxs-lookup"><span data-stu-id="1101e-116">1</span></span>|<span data-ttu-id="1101e-117">Installiert.</span><span class="sxs-lookup"><span data-stu-id="1101e-117">Installed.</span></span>|
|<span data-ttu-id="1101e-118">failed</span><span class="sxs-lookup"><span data-stu-id="1101e-118">failed</span></span>|<span data-ttu-id="1101e-119">2</span><span class="sxs-lookup"><span data-stu-id="1101e-119">2</span></span>|<span data-ttu-id="1101e-120">Fehler bei.</span><span class="sxs-lookup"><span data-stu-id="1101e-120">Failed.</span></span>|
|<span data-ttu-id="1101e-121">notInstalled</span><span class="sxs-lookup"><span data-stu-id="1101e-121">notInstalled</span></span>|<span data-ttu-id="1101e-122">3</span><span class="sxs-lookup"><span data-stu-id="1101e-122">3</span></span>|<span data-ttu-id="1101e-123">Nicht installiert.</span><span class="sxs-lookup"><span data-stu-id="1101e-123">Not Installed.</span></span>|
|<span data-ttu-id="1101e-124">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="1101e-124">uninstallFailed</span></span>|<span data-ttu-id="1101e-125">4</span><span class="sxs-lookup"><span data-stu-id="1101e-125">4</span></span>|<span data-ttu-id="1101e-126">Deinstallieren von ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="1101e-126">Uninstall Failed.</span></span>|
|<span data-ttu-id="1101e-127">unknown</span><span class="sxs-lookup"><span data-stu-id="1101e-127">unknown</span></span>|<span data-ttu-id="1101e-128">5</span><span class="sxs-lookup"><span data-stu-id="1101e-128">5</span></span>|<span data-ttu-id="1101e-129">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="1101e-129">Unknown.</span></span>|





