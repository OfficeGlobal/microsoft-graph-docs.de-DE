---
title: WindowsDeliveryOptimizationMode Enum-Typ
description: Übermittlung Optimierung Modus für Peer-Verteilung
author: tfitzmac
ms.openlocfilehash: ae61d7dde5fc02ff329eaf9cc970ee7078c3a254
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360158"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="ea469-103">WindowsDeliveryOptimizationMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="ea469-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="ea469-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ea469-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea469-105">Übermittlung Optimierung Modus für Peer-Verteilung</span><span class="sxs-lookup"><span data-stu-id="ea469-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="ea469-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="ea469-106">Members</span></span>
|<span data-ttu-id="ea469-107">Member</span><span class="sxs-lookup"><span data-stu-id="ea469-107">Member</span></span>|<span data-ttu-id="ea469-108">Wert</span><span class="sxs-lookup"><span data-stu-id="ea469-108">Value</span></span>|<span data-ttu-id="ea469-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea469-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea469-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="ea469-110">userDefined</span></span>|<span data-ttu-id="ea469-111">0</span><span class="sxs-lookup"><span data-stu-id="ea469-111">0</span></span>|<span data-ttu-id="ea469-112">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="ea469-112">Allow the user to set.</span></span>|
|<span data-ttu-id="ea469-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="ea469-113">httpOnly</span></span>|<span data-ttu-id="ea469-114">1</span><span class="sxs-lookup"><span data-stu-id="ea469-114">1</span></span>|<span data-ttu-id="ea469-115">Nur HTTP keine peering</span><span class="sxs-lookup"><span data-stu-id="ea469-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="ea469-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="ea469-116">httpWithPeeringNat</span></span>|<span data-ttu-id="ea469-117">2</span><span class="sxs-lookup"><span data-stu-id="ea469-117">2</span></span>|<span data-ttu-id="ea469-118">OS Standard – gemischt Http mit hinter den gleichen Network Address Translation peering</span><span class="sxs-lookup"><span data-stu-id="ea469-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="ea469-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="ea469-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="ea469-120">3</span><span class="sxs-lookup"><span data-stu-id="ea469-120">3</span></span>|<span data-ttu-id="ea469-121">HTTP mit über eine private Gruppe peering gemischt</span><span class="sxs-lookup"><span data-stu-id="ea469-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="ea469-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="ea469-122">httpWithInternetPeering</span></span>|<span data-ttu-id="ea469-123">4</span><span class="sxs-lookup"><span data-stu-id="ea469-123">4</span></span>|<span data-ttu-id="ea469-124">HTTP mit Internet peering gemischt</span><span class="sxs-lookup"><span data-stu-id="ea469-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="ea469-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="ea469-125">simpleDownload</span></span>|<span data-ttu-id="ea469-126">99</span><span class="sxs-lookup"><span data-stu-id="ea469-126">99</span></span>|<span data-ttu-id="ea469-127">Einfacher Downloadmodus mit keine peering</span><span class="sxs-lookup"><span data-stu-id="ea469-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="ea469-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="ea469-128">bypassMode</span></span>|<span data-ttu-id="ea469-129">100</span><span class="sxs-lookup"><span data-stu-id="ea469-129">100</span></span>|<span data-ttu-id="ea469-130">Umgehen Sie Modus.</span><span class="sxs-lookup"><span data-stu-id="ea469-130">Bypass mode.</span></span> <span data-ttu-id="ea469-131">Keine verwenden Sie Übermittlung Optimierung und verwenden Sie stattdessen BITS</span><span class="sxs-lookup"><span data-stu-id="ea469-131">Do not use Delivery Optimization and use BITS instead</span></span>|



