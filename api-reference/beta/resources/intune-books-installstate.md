---
title: InstallState Enum-Typ
description: Mögliche Werte für Installationsstatus.
ms.openlocfilehash: c452deb5bc04e944139870d0ccceebc65a91ac1e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059195"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="fe0c9-103">InstallState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="fe0c9-103">installState enum type</span></span>

> <span data-ttu-id="fe0c9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fe0c9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe0c9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fe0c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe0c9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fe0c9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe0c9-107">Mögliche Werte für Installationsstatus.</span><span class="sxs-lookup"><span data-stu-id="fe0c9-107">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="fe0c9-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="fe0c9-108">Members</span></span>
|<span data-ttu-id="fe0c9-109">Element</span><span class="sxs-lookup"><span data-stu-id="fe0c9-109">Member</span></span>|<span data-ttu-id="fe0c9-110">Wert</span><span class="sxs-lookup"><span data-stu-id="fe0c9-110">Value</span></span>|<span data-ttu-id="fe0c9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fe0c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe0c9-112">notApplicable</span><span class="sxs-lookup"><span data-stu-id="fe0c9-112">notApplicable</span></span>|<span data-ttu-id="fe0c9-113">0</span><span class="sxs-lookup"><span data-stu-id="fe0c9-113">0</span></span>|<span data-ttu-id="fe0c9-114">Nicht zutreffend.</span><span class="sxs-lookup"><span data-stu-id="fe0c9-114">Not Applicable.</span></span>|
|<span data-ttu-id="fe0c9-115">installiert</span><span class="sxs-lookup"><span data-stu-id="fe0c9-115">installed</span></span>|<span data-ttu-id="fe0c9-116">1</span><span class="sxs-lookup"><span data-stu-id="fe0c9-116">1</span></span>|<span data-ttu-id="fe0c9-117">Installiert.</span><span class="sxs-lookup"><span data-stu-id="fe0c9-117">Installed.</span></span>|
|<span data-ttu-id="fe0c9-118">failed</span><span class="sxs-lookup"><span data-stu-id="fe0c9-118">failed</span></span>|<span data-ttu-id="fe0c9-119">2</span><span class="sxs-lookup"><span data-stu-id="fe0c9-119">2</span></span>|<span data-ttu-id="fe0c9-120">Fehler bei.</span><span class="sxs-lookup"><span data-stu-id="fe0c9-120">Failed.</span></span>|
|<span data-ttu-id="fe0c9-121">notInstalled</span><span class="sxs-lookup"><span data-stu-id="fe0c9-121">notInstalled</span></span>|<span data-ttu-id="fe0c9-122">3</span><span class="sxs-lookup"><span data-stu-id="fe0c9-122">3</span></span>|<span data-ttu-id="fe0c9-123">Nicht installiert.</span><span class="sxs-lookup"><span data-stu-id="fe0c9-123">Not Installed.</span></span>|
|<span data-ttu-id="fe0c9-124">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="fe0c9-124">uninstallFailed</span></span>|<span data-ttu-id="fe0c9-125">4</span><span class="sxs-lookup"><span data-stu-id="fe0c9-125">4</span></span>|<span data-ttu-id="fe0c9-126">Deinstallieren von ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="fe0c9-126">Uninstall Failed.</span></span>|
|<span data-ttu-id="fe0c9-127">unknown</span><span class="sxs-lookup"><span data-stu-id="fe0c9-127">unknown</span></span>|<span data-ttu-id="fe0c9-128">5</span><span class="sxs-lookup"><span data-stu-id="fe0c9-128">5</span></span>|<span data-ttu-id="fe0c9-129">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="fe0c9-129">Unknown.</span></span>|





