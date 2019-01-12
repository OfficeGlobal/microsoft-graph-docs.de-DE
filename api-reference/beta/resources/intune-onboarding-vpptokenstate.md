---
title: VppTokenState Enum-Typ
description: Möglichen Zuständen ein Token Apple Volume Purchase Program zugeordnet.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b8e2148cccbb891b1c139abd9d15ba424b3b3e9b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967378"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="a2aef-103">VppTokenState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="a2aef-103">vppTokenState enum type</span></span>

> <span data-ttu-id="a2aef-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a2aef-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2aef-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a2aef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2aef-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a2aef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2aef-107">Möglichen Zuständen ein Token Apple Volume Purchase Program zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="a2aef-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="a2aef-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="a2aef-108">Members</span></span>
|<span data-ttu-id="a2aef-109">Element</span><span class="sxs-lookup"><span data-stu-id="a2aef-109">Member</span></span>|<span data-ttu-id="a2aef-110">Wert</span><span class="sxs-lookup"><span data-stu-id="a2aef-110">Value</span></span>|<span data-ttu-id="a2aef-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a2aef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2aef-112">unknown</span><span class="sxs-lookup"><span data-stu-id="a2aef-112">unknown</span></span>|<span data-ttu-id="a2aef-113">0</span><span class="sxs-lookup"><span data-stu-id="a2aef-113">0</span></span>|<span data-ttu-id="a2aef-114">Standardzustand.</span><span class="sxs-lookup"><span data-stu-id="a2aef-114">Default state.</span></span>|
|<span data-ttu-id="a2aef-115">gültige</span><span class="sxs-lookup"><span data-stu-id="a2aef-115">valid</span></span>|<span data-ttu-id="a2aef-116">1</span><span class="sxs-lookup"><span data-stu-id="a2aef-116">1</span></span>|<span data-ttu-id="a2aef-117">Das Token ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="a2aef-117">Token is valid.</span></span>|
|<span data-ttu-id="a2aef-118">abgelaufen</span><span class="sxs-lookup"><span data-stu-id="a2aef-118">expired</span></span>|<span data-ttu-id="a2aef-119">2</span><span class="sxs-lookup"><span data-stu-id="a2aef-119">2</span></span>|<span data-ttu-id="a2aef-120">Token ist abgelaufen.</span><span class="sxs-lookup"><span data-stu-id="a2aef-120">Token is expired.</span></span>|
|<span data-ttu-id="a2aef-121">Ungültig</span><span class="sxs-lookup"><span data-stu-id="a2aef-121">invalid</span></span>|<span data-ttu-id="a2aef-122">3</span><span class="sxs-lookup"><span data-stu-id="a2aef-122">3</span></span>|<span data-ttu-id="a2aef-123">Token ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="a2aef-123">Token is invalid.</span></span>|
|<span data-ttu-id="a2aef-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="a2aef-124">assignedToExternalMDM</span></span>|<span data-ttu-id="a2aef-125">4</span><span class="sxs-lookup"><span data-stu-id="a2aef-125">4</span></span>|<span data-ttu-id="a2aef-126">Token wird von einem anderen MDM-Dienst verwaltet.</span><span class="sxs-lookup"><span data-stu-id="a2aef-126">Token is managed by another MDM Service.</span></span>|





