---
title: VppTokenState Enum-Typ
description: Möglichen Zuständen ein Token Apple Volume Purchase Program zugeordnet.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6bdeb73b6491f3960ce30db91a35d06c0f8ffaf1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986663"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="ac04d-103">VppTokenState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="ac04d-103">vppTokenState enum type</span></span>

> <span data-ttu-id="ac04d-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ac04d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac04d-105">Möglichen Zuständen ein Token Apple Volume Purchase Program zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="ac04d-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="ac04d-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="ac04d-106">Members</span></span>
|<span data-ttu-id="ac04d-107">Element</span><span class="sxs-lookup"><span data-stu-id="ac04d-107">Member</span></span>|<span data-ttu-id="ac04d-108">Wert</span><span class="sxs-lookup"><span data-stu-id="ac04d-108">Value</span></span>|<span data-ttu-id="ac04d-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac04d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac04d-110">unknown</span><span class="sxs-lookup"><span data-stu-id="ac04d-110">unknown</span></span>|<span data-ttu-id="ac04d-111">0</span><span class="sxs-lookup"><span data-stu-id="ac04d-111">0</span></span>|<span data-ttu-id="ac04d-112">Standardzustand.</span><span class="sxs-lookup"><span data-stu-id="ac04d-112">Default state.</span></span>|
|<span data-ttu-id="ac04d-113">gültige</span><span class="sxs-lookup"><span data-stu-id="ac04d-113">valid</span></span>|<span data-ttu-id="ac04d-114">1</span><span class="sxs-lookup"><span data-stu-id="ac04d-114">1</span></span>|<span data-ttu-id="ac04d-115">Das Token ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="ac04d-115">Token is valid.</span></span>|
|<span data-ttu-id="ac04d-116">abgelaufen</span><span class="sxs-lookup"><span data-stu-id="ac04d-116">expired</span></span>|<span data-ttu-id="ac04d-117">2</span><span class="sxs-lookup"><span data-stu-id="ac04d-117">2</span></span>|<span data-ttu-id="ac04d-118">Token ist abgelaufen.</span><span class="sxs-lookup"><span data-stu-id="ac04d-118">Token is expired.</span></span>|
|<span data-ttu-id="ac04d-119">Ungültig</span><span class="sxs-lookup"><span data-stu-id="ac04d-119">invalid</span></span>|<span data-ttu-id="ac04d-120">3</span><span class="sxs-lookup"><span data-stu-id="ac04d-120">3</span></span>|<span data-ttu-id="ac04d-121">Token ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="ac04d-121">Token is invalid.</span></span>|
|<span data-ttu-id="ac04d-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="ac04d-122">assignedToExternalMDM</span></span>|<span data-ttu-id="ac04d-123">4</span><span class="sxs-lookup"><span data-stu-id="ac04d-123">4</span></span>|<span data-ttu-id="ac04d-124">Token wird von einem anderen MDM-Dienst verwaltet.</span><span class="sxs-lookup"><span data-stu-id="ac04d-124">Token is managed by another MDM Service.</span></span>|



