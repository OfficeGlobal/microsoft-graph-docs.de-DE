---
title: WindowsDeliveryOptimizationMode Enum-Typ
description: Übermittlung Optimierung Modus für Peer-Verteilung
ms.openlocfilehash: 2d393a82f855f3e3a0226c8ccb450fa2dae1a95c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017405"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="fb581-103">WindowsDeliveryOptimizationMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="fb581-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="fb581-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fb581-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb581-105">Übermittlung Optimierung Modus für Peer-Verteilung</span><span class="sxs-lookup"><span data-stu-id="fb581-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="fb581-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="fb581-106">Members</span></span>
|<span data-ttu-id="fb581-107">Element</span><span class="sxs-lookup"><span data-stu-id="fb581-107">Member</span></span>|<span data-ttu-id="fb581-108">Wert</span><span class="sxs-lookup"><span data-stu-id="fb581-108">Value</span></span>|<span data-ttu-id="fb581-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fb581-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb581-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="fb581-110">userDefined</span></span>|<span data-ttu-id="fb581-111">0</span><span class="sxs-lookup"><span data-stu-id="fb581-111">0</span></span>|<span data-ttu-id="fb581-112">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="fb581-112">Allow the user to set.</span></span>|
|<span data-ttu-id="fb581-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="fb581-113">httpOnly</span></span>|<span data-ttu-id="fb581-114">1</span><span class="sxs-lookup"><span data-stu-id="fb581-114">1</span></span>|<span data-ttu-id="fb581-115">Nur HTTP keine peering</span><span class="sxs-lookup"><span data-stu-id="fb581-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="fb581-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="fb581-116">httpWithPeeringNat</span></span>|<span data-ttu-id="fb581-117">2</span><span class="sxs-lookup"><span data-stu-id="fb581-117">2</span></span>|<span data-ttu-id="fb581-118">OS Standard – gemischt Http mit hinter den gleichen Network Address Translation peering</span><span class="sxs-lookup"><span data-stu-id="fb581-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="fb581-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="fb581-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="fb581-120">3</span><span class="sxs-lookup"><span data-stu-id="fb581-120">3</span></span>|<span data-ttu-id="fb581-121">HTTP mit über eine private Gruppe peering gemischt</span><span class="sxs-lookup"><span data-stu-id="fb581-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="fb581-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="fb581-122">httpWithInternetPeering</span></span>|<span data-ttu-id="fb581-123">4</span><span class="sxs-lookup"><span data-stu-id="fb581-123">4</span></span>|<span data-ttu-id="fb581-124">HTTP mit Internet peering gemischt</span><span class="sxs-lookup"><span data-stu-id="fb581-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="fb581-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="fb581-125">simpleDownload</span></span>|<span data-ttu-id="fb581-126">99</span><span class="sxs-lookup"><span data-stu-id="fb581-126">99</span></span>|<span data-ttu-id="fb581-127">Einfacher Downloadmodus mit keine peering</span><span class="sxs-lookup"><span data-stu-id="fb581-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="fb581-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="fb581-128">bypassMode</span></span>|<span data-ttu-id="fb581-129">100</span><span class="sxs-lookup"><span data-stu-id="fb581-129">100</span></span>|<span data-ttu-id="fb581-130">Umgehen Sie Modus.</span><span class="sxs-lookup"><span data-stu-id="fb581-130">Bypass mode.</span></span> <span data-ttu-id="fb581-131">Keine verwenden Sie Übermittlung Optimierung und verwenden Sie stattdessen BITS</span><span class="sxs-lookup"><span data-stu-id="fb581-131">Do not use Delivery Optimization and use BITS instead</span></span>|



