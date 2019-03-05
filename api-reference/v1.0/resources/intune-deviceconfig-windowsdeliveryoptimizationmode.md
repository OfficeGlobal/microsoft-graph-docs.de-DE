---
title: windowsDeliveryOptimizationMode-Enumerationstyp
description: Bereitstellungs Optimierungsmodus für die Peer Verteilung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9034c7c90257a7ca622cd203d4ab84387fd2014
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251503"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="baa8e-103">windowsDeliveryOptimizationMode-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="baa8e-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="baa8e-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="baa8e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="baa8e-105">Bereitstellungs Optimierungsmodus für die Peer Verteilung</span><span class="sxs-lookup"><span data-stu-id="baa8e-105">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="baa8e-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="baa8e-106">Members</span></span>
|<span data-ttu-id="baa8e-107">Element</span><span class="sxs-lookup"><span data-stu-id="baa8e-107">Member</span></span>|<span data-ttu-id="baa8e-108">Wert</span><span class="sxs-lookup"><span data-stu-id="baa8e-108">Value</span></span>|<span data-ttu-id="baa8e-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="baa8e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baa8e-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="baa8e-110">userDefined</span></span>|<span data-ttu-id="baa8e-111">0</span><span class="sxs-lookup"><span data-stu-id="baa8e-111">0</span></span>|<span data-ttu-id="baa8e-112">Zulassen, dass der Benutzer festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="baa8e-112">Allow the user to set.</span></span>|
|<span data-ttu-id="baa8e-113">"HttpOnly"</span><span class="sxs-lookup"><span data-stu-id="baa8e-113">httpOnly</span></span>|<span data-ttu-id="baa8e-114">1</span><span class="sxs-lookup"><span data-stu-id="baa8e-114">1</span></span>|<span data-ttu-id="baa8e-115">Nur HTTP, kein Peering</span><span class="sxs-lookup"><span data-stu-id="baa8e-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="baa8e-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="baa8e-116">httpWithPeeringNat</span></span>|<span data-ttu-id="baa8e-117">2</span><span class="sxs-lookup"><span data-stu-id="baa8e-117">2</span></span>|<span data-ttu-id="baa8e-118">Betriebssystemstandard – http-Überblendung mit Peering hinter demselben Netzwerkadressübersetzer</span><span class="sxs-lookup"><span data-stu-id="baa8e-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="baa8e-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="baa8e-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="baa8e-120">3</span><span class="sxs-lookup"><span data-stu-id="baa8e-120">3</span></span>|<span data-ttu-id="baa8e-121">HTTP-Überblendung mit Peering über eine private Gruppe hinweg</span><span class="sxs-lookup"><span data-stu-id="baa8e-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="baa8e-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="baa8e-122">httpWithInternetPeering</span></span>|<span data-ttu-id="baa8e-123">4</span><span class="sxs-lookup"><span data-stu-id="baa8e-123">4</span></span>|<span data-ttu-id="baa8e-124">HTTP-Blended mit Internet-Peering</span><span class="sxs-lookup"><span data-stu-id="baa8e-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="baa8e-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="baa8e-125">simpleDownload</span></span>|<span data-ttu-id="baa8e-126">99</span><span class="sxs-lookup"><span data-stu-id="baa8e-126">99</span></span>|<span data-ttu-id="baa8e-127">Einfacher Downloadmodus ohne Peering</span><span class="sxs-lookup"><span data-stu-id="baa8e-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="baa8e-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="baa8e-128">bypassMode</span></span>|<span data-ttu-id="baa8e-129">100</span><span class="sxs-lookup"><span data-stu-id="baa8e-129">100</span></span>|<span data-ttu-id="baa8e-130">Umgehungsmodus.</span><span class="sxs-lookup"><span data-stu-id="baa8e-130">Bypass mode.</span></span> <span data-ttu-id="baa8e-131">Verwenden Sie keine BereitstellungsOptimierung und verwenden Sie stattdessen BITS.</span><span class="sxs-lookup"><span data-stu-id="baa8e-131">Do not use Delivery Optimization and use BITS instead</span></span>|



