---
title: InstallState Enum-Typ
description: Mögliche Werte für Installationsstatus.
author: tfitzmac
ms.openlocfilehash: c8e1a6ef50574eaa6f704e1d9f49d56c83046ab7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304634"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="ce801-103">InstallState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="ce801-103">installState enum type</span></span>

> <span data-ttu-id="ce801-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ce801-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce801-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ce801-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce801-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ce801-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce801-107">Mögliche Werte für Installationsstatus.</span><span class="sxs-lookup"><span data-stu-id="ce801-107">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="ce801-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="ce801-108">Members</span></span>
|<span data-ttu-id="ce801-109">Member</span><span class="sxs-lookup"><span data-stu-id="ce801-109">Member</span></span>|<span data-ttu-id="ce801-110">Wert</span><span class="sxs-lookup"><span data-stu-id="ce801-110">Value</span></span>|<span data-ttu-id="ce801-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce801-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce801-112">notApplicable</span><span class="sxs-lookup"><span data-stu-id="ce801-112">notApplicable</span></span>|<span data-ttu-id="ce801-113">0</span><span class="sxs-lookup"><span data-stu-id="ce801-113">0</span></span>|<span data-ttu-id="ce801-114">Nicht zutreffend.</span><span class="sxs-lookup"><span data-stu-id="ce801-114">Not Applicable.</span></span>|
|<span data-ttu-id="ce801-115">installiert</span><span class="sxs-lookup"><span data-stu-id="ce801-115">installed</span></span>|<span data-ttu-id="ce801-116">1</span><span class="sxs-lookup"><span data-stu-id="ce801-116">1</span></span>|<span data-ttu-id="ce801-117">Installiert.</span><span class="sxs-lookup"><span data-stu-id="ce801-117">Installed.</span></span>|
|<span data-ttu-id="ce801-118">failed</span><span class="sxs-lookup"><span data-stu-id="ce801-118">failed</span></span>|<span data-ttu-id="ce801-119">2</span><span class="sxs-lookup"><span data-stu-id="ce801-119">2</span></span>|<span data-ttu-id="ce801-120">Fehler bei.</span><span class="sxs-lookup"><span data-stu-id="ce801-120">Failed.</span></span>|
|<span data-ttu-id="ce801-121">notInstalled</span><span class="sxs-lookup"><span data-stu-id="ce801-121">notInstalled</span></span>|<span data-ttu-id="ce801-122">3</span><span class="sxs-lookup"><span data-stu-id="ce801-122">3</span></span>|<span data-ttu-id="ce801-123">Nicht installiert.</span><span class="sxs-lookup"><span data-stu-id="ce801-123">Not Installed.</span></span>|
|<span data-ttu-id="ce801-124">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="ce801-124">uninstallFailed</span></span>|<span data-ttu-id="ce801-125">4</span><span class="sxs-lookup"><span data-stu-id="ce801-125">4</span></span>|<span data-ttu-id="ce801-126">Deinstallieren von ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="ce801-126">Uninstall Failed.</span></span>|
|<span data-ttu-id="ce801-127">unknown</span><span class="sxs-lookup"><span data-stu-id="ce801-127">unknown</span></span>|<span data-ttu-id="ce801-128">5</span><span class="sxs-lookup"><span data-stu-id="ce801-128">5</span></span>|<span data-ttu-id="ce801-129">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="ce801-129">Unknown.</span></span>|





