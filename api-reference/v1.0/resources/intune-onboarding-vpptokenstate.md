---
title: VppTokenState Enum-Typ
description: Möglichen Zuständen ein Token Apple Volume Purchase Program zugeordnet.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 89d28a07bb2c6abea2e2a10d9b5a0961e5efecff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834027"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="7363e-103">VppTokenState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="7363e-103">vppTokenState enum type</span></span>

> <span data-ttu-id="7363e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7363e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7363e-105">Möglichen Zuständen ein Token Apple Volume Purchase Program zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="7363e-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="7363e-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="7363e-106">Members</span></span>
|<span data-ttu-id="7363e-107">Element</span><span class="sxs-lookup"><span data-stu-id="7363e-107">Member</span></span>|<span data-ttu-id="7363e-108">Wert</span><span class="sxs-lookup"><span data-stu-id="7363e-108">Value</span></span>|<span data-ttu-id="7363e-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7363e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7363e-110">unknown</span><span class="sxs-lookup"><span data-stu-id="7363e-110">unknown</span></span>|<span data-ttu-id="7363e-111">0</span><span class="sxs-lookup"><span data-stu-id="7363e-111">0</span></span>|<span data-ttu-id="7363e-112">Standardzustand.</span><span class="sxs-lookup"><span data-stu-id="7363e-112">Default state.</span></span>|
|<span data-ttu-id="7363e-113">gültige</span><span class="sxs-lookup"><span data-stu-id="7363e-113">valid</span></span>|<span data-ttu-id="7363e-114">1</span><span class="sxs-lookup"><span data-stu-id="7363e-114">1</span></span>|<span data-ttu-id="7363e-115">Das Token ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="7363e-115">Token is valid.</span></span>|
|<span data-ttu-id="7363e-116">abgelaufen</span><span class="sxs-lookup"><span data-stu-id="7363e-116">expired</span></span>|<span data-ttu-id="7363e-117">2</span><span class="sxs-lookup"><span data-stu-id="7363e-117">2</span></span>|<span data-ttu-id="7363e-118">Token ist abgelaufen.</span><span class="sxs-lookup"><span data-stu-id="7363e-118">Token is expired.</span></span>|
|<span data-ttu-id="7363e-119">Ungültig</span><span class="sxs-lookup"><span data-stu-id="7363e-119">invalid</span></span>|<span data-ttu-id="7363e-120">3</span><span class="sxs-lookup"><span data-stu-id="7363e-120">3</span></span>|<span data-ttu-id="7363e-121">Token ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="7363e-121">Token is invalid.</span></span>|
|<span data-ttu-id="7363e-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="7363e-122">assignedToExternalMDM</span></span>|<span data-ttu-id="7363e-123">4</span><span class="sxs-lookup"><span data-stu-id="7363e-123">4</span></span>|<span data-ttu-id="7363e-124">Token wird von einem anderen MDM-Dienst verwaltet.</span><span class="sxs-lookup"><span data-stu-id="7363e-124">Token is managed by another MDM Service.</span></span>|



