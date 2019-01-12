---
title: InstallState Enum-Typ
description: Mögliche Werte für Installationsstatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b50fb44c2af31efff81f2dd7097505f71bc791d5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947549"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="a5786-103">InstallState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="a5786-103">installState enum type</span></span>

> <span data-ttu-id="a5786-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a5786-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5786-105">Mögliche Werte für Installationsstatus.</span><span class="sxs-lookup"><span data-stu-id="a5786-105">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="a5786-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="a5786-106">Members</span></span>
|<span data-ttu-id="a5786-107">Element</span><span class="sxs-lookup"><span data-stu-id="a5786-107">Member</span></span>|<span data-ttu-id="a5786-108">Wert</span><span class="sxs-lookup"><span data-stu-id="a5786-108">Value</span></span>|<span data-ttu-id="a5786-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5786-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5786-110">notApplicable</span><span class="sxs-lookup"><span data-stu-id="a5786-110">notApplicable</span></span>|<span data-ttu-id="a5786-111">0</span><span class="sxs-lookup"><span data-stu-id="a5786-111">0</span></span>|<span data-ttu-id="a5786-112">Nicht zutreffend.</span><span class="sxs-lookup"><span data-stu-id="a5786-112">Not Applicable.</span></span>|
|<span data-ttu-id="a5786-113">installiert</span><span class="sxs-lookup"><span data-stu-id="a5786-113">installed</span></span>|<span data-ttu-id="a5786-114">1</span><span class="sxs-lookup"><span data-stu-id="a5786-114">1</span></span>|<span data-ttu-id="a5786-115">Installiert.</span><span class="sxs-lookup"><span data-stu-id="a5786-115">Installed.</span></span>|
|<span data-ttu-id="a5786-116">failed</span><span class="sxs-lookup"><span data-stu-id="a5786-116">failed</span></span>|<span data-ttu-id="a5786-117">2</span><span class="sxs-lookup"><span data-stu-id="a5786-117">2</span></span>|<span data-ttu-id="a5786-118">Fehler bei.</span><span class="sxs-lookup"><span data-stu-id="a5786-118">Failed.</span></span>|
|<span data-ttu-id="a5786-119">notInstalled</span><span class="sxs-lookup"><span data-stu-id="a5786-119">notInstalled</span></span>|<span data-ttu-id="a5786-120">3</span><span class="sxs-lookup"><span data-stu-id="a5786-120">3</span></span>|<span data-ttu-id="a5786-121">Nicht installiert.</span><span class="sxs-lookup"><span data-stu-id="a5786-121">Not Installed.</span></span>|
|<span data-ttu-id="a5786-122">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="a5786-122">uninstallFailed</span></span>|<span data-ttu-id="a5786-123">4</span><span class="sxs-lookup"><span data-stu-id="a5786-123">4</span></span>|<span data-ttu-id="a5786-124">Deinstallieren von ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="a5786-124">Uninstall Failed.</span></span>|
|<span data-ttu-id="a5786-125">unknown</span><span class="sxs-lookup"><span data-stu-id="a5786-125">unknown</span></span>|<span data-ttu-id="a5786-126">5</span><span class="sxs-lookup"><span data-stu-id="a5786-126">5</span></span>|<span data-ttu-id="a5786-127">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="a5786-127">Unknown.</span></span>|



