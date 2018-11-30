---
title: WindowsDeliveryOptimizationMode Enum-Typ
description: Übermittlung Optimierung Modus für Peer-Verteilung
ms.openlocfilehash: 99795f3d901b538990d4dfec7a426e66794c5946
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060577"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="19b82-103">WindowsDeliveryOptimizationMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="19b82-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="19b82-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="19b82-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19b82-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19b82-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19b82-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="19b82-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19b82-107">Übermittlung Optimierung Modus für Peer-Verteilung</span><span class="sxs-lookup"><span data-stu-id="19b82-107">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="19b82-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="19b82-108">Members</span></span>
|<span data-ttu-id="19b82-109">Element</span><span class="sxs-lookup"><span data-stu-id="19b82-109">Member</span></span>|<span data-ttu-id="19b82-110">Wert</span><span class="sxs-lookup"><span data-stu-id="19b82-110">Value</span></span>|<span data-ttu-id="19b82-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19b82-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19b82-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="19b82-112">userDefined</span></span>|<span data-ttu-id="19b82-113">0</span><span class="sxs-lookup"><span data-stu-id="19b82-113">0</span></span>|<span data-ttu-id="19b82-114">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="19b82-114">Allow the user to set.</span></span>|
|<span data-ttu-id="19b82-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="19b82-115">httpOnly</span></span>|<span data-ttu-id="19b82-116">1</span><span class="sxs-lookup"><span data-stu-id="19b82-116">1</span></span>|<span data-ttu-id="19b82-117">Nur HTTP keine peering</span><span class="sxs-lookup"><span data-stu-id="19b82-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="19b82-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="19b82-118">httpWithPeeringNat</span></span>|<span data-ttu-id="19b82-119">2</span><span class="sxs-lookup"><span data-stu-id="19b82-119">2</span></span>|<span data-ttu-id="19b82-120">OS Standard – gemischt Http mit hinter den gleichen Network Address Translation peering</span><span class="sxs-lookup"><span data-stu-id="19b82-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="19b82-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="19b82-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="19b82-122">3</span><span class="sxs-lookup"><span data-stu-id="19b82-122">3</span></span>|<span data-ttu-id="19b82-123">HTTP mit über eine private Gruppe peering gemischt</span><span class="sxs-lookup"><span data-stu-id="19b82-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="19b82-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="19b82-124">httpWithInternetPeering</span></span>|<span data-ttu-id="19b82-125">4</span><span class="sxs-lookup"><span data-stu-id="19b82-125">4</span></span>|<span data-ttu-id="19b82-126">HTTP mit Internet peering gemischt</span><span class="sxs-lookup"><span data-stu-id="19b82-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="19b82-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="19b82-127">simpleDownload</span></span>|<span data-ttu-id="19b82-128">99</span><span class="sxs-lookup"><span data-stu-id="19b82-128">99</span></span>|<span data-ttu-id="19b82-129">Einfacher Downloadmodus mit keine peering</span><span class="sxs-lookup"><span data-stu-id="19b82-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="19b82-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="19b82-130">bypassMode</span></span>|<span data-ttu-id="19b82-131">100</span><span class="sxs-lookup"><span data-stu-id="19b82-131">100</span></span>|<span data-ttu-id="19b82-132">Umgehen Sie Modus.</span><span class="sxs-lookup"><span data-stu-id="19b82-132">Bypass mode.</span></span> <span data-ttu-id="19b82-133">Keine verwenden Sie Übermittlung Optimierung und verwenden Sie stattdessen BITS</span><span class="sxs-lookup"><span data-stu-id="19b82-133">Do not use Delivery Optimization and use BITS instead</span></span>|





