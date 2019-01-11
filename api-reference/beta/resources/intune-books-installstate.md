---
title: InstallState Enum-Typ
description: Mögliche Werte für Installationsstatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fa281cc5f218469980a235db842e00fd8fa46647
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868621"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="4b40c-103">InstallState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="4b40c-103">installState enum type</span></span>

> <span data-ttu-id="4b40c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4b40c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b40c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b40c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b40c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4b40c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b40c-107">Mögliche Werte für Installationsstatus.</span><span class="sxs-lookup"><span data-stu-id="4b40c-107">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="4b40c-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="4b40c-108">Members</span></span>
|<span data-ttu-id="4b40c-109">Element</span><span class="sxs-lookup"><span data-stu-id="4b40c-109">Member</span></span>|<span data-ttu-id="4b40c-110">Wert</span><span class="sxs-lookup"><span data-stu-id="4b40c-110">Value</span></span>|<span data-ttu-id="4b40c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b40c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b40c-112">notApplicable</span><span class="sxs-lookup"><span data-stu-id="4b40c-112">notApplicable</span></span>|<span data-ttu-id="4b40c-113">0</span><span class="sxs-lookup"><span data-stu-id="4b40c-113">0</span></span>|<span data-ttu-id="4b40c-114">Nicht zutreffend.</span><span class="sxs-lookup"><span data-stu-id="4b40c-114">Not Applicable.</span></span>|
|<span data-ttu-id="4b40c-115">installiert</span><span class="sxs-lookup"><span data-stu-id="4b40c-115">installed</span></span>|<span data-ttu-id="4b40c-116">1</span><span class="sxs-lookup"><span data-stu-id="4b40c-116">1</span></span>|<span data-ttu-id="4b40c-117">Installiert.</span><span class="sxs-lookup"><span data-stu-id="4b40c-117">Installed.</span></span>|
|<span data-ttu-id="4b40c-118">failed</span><span class="sxs-lookup"><span data-stu-id="4b40c-118">failed</span></span>|<span data-ttu-id="4b40c-119">2</span><span class="sxs-lookup"><span data-stu-id="4b40c-119">2</span></span>|<span data-ttu-id="4b40c-120">Fehler bei.</span><span class="sxs-lookup"><span data-stu-id="4b40c-120">Failed.</span></span>|
|<span data-ttu-id="4b40c-121">notInstalled</span><span class="sxs-lookup"><span data-stu-id="4b40c-121">notInstalled</span></span>|<span data-ttu-id="4b40c-122">3</span><span class="sxs-lookup"><span data-stu-id="4b40c-122">3</span></span>|<span data-ttu-id="4b40c-123">Nicht installiert.</span><span class="sxs-lookup"><span data-stu-id="4b40c-123">Not Installed.</span></span>|
|<span data-ttu-id="4b40c-124">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="4b40c-124">uninstallFailed</span></span>|<span data-ttu-id="4b40c-125">4</span><span class="sxs-lookup"><span data-stu-id="4b40c-125">4</span></span>|<span data-ttu-id="4b40c-126">Deinstallieren von ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="4b40c-126">Uninstall Failed.</span></span>|
|<span data-ttu-id="4b40c-127">unknown</span><span class="sxs-lookup"><span data-stu-id="4b40c-127">unknown</span></span>|<span data-ttu-id="4b40c-128">5</span><span class="sxs-lookup"><span data-stu-id="4b40c-128">5</span></span>|<span data-ttu-id="4b40c-129">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="4b40c-129">Unknown.</span></span>|





