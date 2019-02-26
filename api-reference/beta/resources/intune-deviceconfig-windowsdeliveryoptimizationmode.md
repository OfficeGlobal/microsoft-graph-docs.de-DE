---
title: windowsDeliveryOptimizationMode-Enumerationstyp
description: Bereitstellungs Optimierungsmodus für die Peer Verteilung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a4b0860e05d20ea480f9c91264033f7a9eb41a0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149168"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="2d596-103">windowsDeliveryOptimizationMode-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="2d596-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="2d596-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2d596-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d596-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2d596-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d596-106">Bereitstellungs Optimierungsmodus für die Peer Verteilung</span><span class="sxs-lookup"><span data-stu-id="2d596-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="2d596-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="2d596-107">Members</span></span>
|<span data-ttu-id="2d596-108">Element</span><span class="sxs-lookup"><span data-stu-id="2d596-108">Member</span></span>|<span data-ttu-id="2d596-109">Wert</span><span class="sxs-lookup"><span data-stu-id="2d596-109">Value</span></span>|<span data-ttu-id="2d596-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2d596-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d596-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="2d596-111">userDefined</span></span>|<span data-ttu-id="2d596-112">0</span><span class="sxs-lookup"><span data-stu-id="2d596-112">0</span></span>|<span data-ttu-id="2d596-113">Zulassen, dass der Benutzer festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="2d596-113">Allow the user to set.</span></span>|
|<span data-ttu-id="2d596-114">"HttpOnly"</span><span class="sxs-lookup"><span data-stu-id="2d596-114">httpOnly</span></span>|<span data-ttu-id="2d596-115">1</span><span class="sxs-lookup"><span data-stu-id="2d596-115">1</span></span>|<span data-ttu-id="2d596-116">Nur HTTP, kein Peering</span><span class="sxs-lookup"><span data-stu-id="2d596-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="2d596-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="2d596-117">httpWithPeeringNat</span></span>|<span data-ttu-id="2d596-118">2</span><span class="sxs-lookup"><span data-stu-id="2d596-118">2</span></span>|<span data-ttu-id="2d596-119">Betriebssystemstandard – http-Überblendung mit Peering hinter demselben Netzwerkadressübersetzer</span><span class="sxs-lookup"><span data-stu-id="2d596-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="2d596-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="2d596-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="2d596-121">3</span><span class="sxs-lookup"><span data-stu-id="2d596-121">3</span></span>|<span data-ttu-id="2d596-122">HTTP-Überblendung mit Peering über eine private Gruppe hinweg</span><span class="sxs-lookup"><span data-stu-id="2d596-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="2d596-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="2d596-123">httpWithInternetPeering</span></span>|<span data-ttu-id="2d596-124">4</span><span class="sxs-lookup"><span data-stu-id="2d596-124">4</span></span>|<span data-ttu-id="2d596-125">HTTP-Blended mit Internet-Peering</span><span class="sxs-lookup"><span data-stu-id="2d596-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="2d596-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="2d596-126">simpleDownload</span></span>|<span data-ttu-id="2d596-127">99</span><span class="sxs-lookup"><span data-stu-id="2d596-127">99</span></span>|<span data-ttu-id="2d596-128">Einfacher Downloadmodus ohne Peering</span><span class="sxs-lookup"><span data-stu-id="2d596-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="2d596-129">bypassMode</span><span class="sxs-lookup"><span data-stu-id="2d596-129">bypassMode</span></span>|<span data-ttu-id="2d596-130">100</span><span class="sxs-lookup"><span data-stu-id="2d596-130">100</span></span>|<span data-ttu-id="2d596-131">Umgehungsmodus.</span><span class="sxs-lookup"><span data-stu-id="2d596-131">Bypass mode.</span></span> <span data-ttu-id="2d596-132">Verwenden Sie keine BereitstellungsOptimierung und verwenden Sie stattdessen BITS.</span><span class="sxs-lookup"><span data-stu-id="2d596-132">Do not use Delivery Optimization and use BITS instead</span></span>|




