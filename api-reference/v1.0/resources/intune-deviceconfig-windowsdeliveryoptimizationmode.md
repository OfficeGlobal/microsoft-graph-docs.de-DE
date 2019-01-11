---
title: WindowsDeliveryOptimizationMode Enum-Typ
description: Übermittlung Optimierung Modus für Peer-Verteilung
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af266b55fd58f788965d33d0d807511d263f6195
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888179"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="e75c9-103">WindowsDeliveryOptimizationMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="e75c9-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="e75c9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e75c9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e75c9-105">Übermittlung Optimierung Modus für Peer-Verteilung</span><span class="sxs-lookup"><span data-stu-id="e75c9-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="e75c9-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="e75c9-106">Members</span></span>
|<span data-ttu-id="e75c9-107">Element</span><span class="sxs-lookup"><span data-stu-id="e75c9-107">Member</span></span>|<span data-ttu-id="e75c9-108">Wert</span><span class="sxs-lookup"><span data-stu-id="e75c9-108">Value</span></span>|<span data-ttu-id="e75c9-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e75c9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e75c9-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="e75c9-110">userDefined</span></span>|<span data-ttu-id="e75c9-111">0</span><span class="sxs-lookup"><span data-stu-id="e75c9-111">0</span></span>|<span data-ttu-id="e75c9-112">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="e75c9-112">Allow the user to set.</span></span>|
|<span data-ttu-id="e75c9-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="e75c9-113">httpOnly</span></span>|<span data-ttu-id="e75c9-114">1</span><span class="sxs-lookup"><span data-stu-id="e75c9-114">1</span></span>|<span data-ttu-id="e75c9-115">Nur HTTP keine peering</span><span class="sxs-lookup"><span data-stu-id="e75c9-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="e75c9-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="e75c9-116">httpWithPeeringNat</span></span>|<span data-ttu-id="e75c9-117">2</span><span class="sxs-lookup"><span data-stu-id="e75c9-117">2</span></span>|<span data-ttu-id="e75c9-118">OS Standard – gemischt Http mit hinter den gleichen Network Address Translation peering</span><span class="sxs-lookup"><span data-stu-id="e75c9-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="e75c9-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="e75c9-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="e75c9-120">3</span><span class="sxs-lookup"><span data-stu-id="e75c9-120">3</span></span>|<span data-ttu-id="e75c9-121">HTTP mit über eine private Gruppe peering gemischt</span><span class="sxs-lookup"><span data-stu-id="e75c9-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="e75c9-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="e75c9-122">httpWithInternetPeering</span></span>|<span data-ttu-id="e75c9-123">4</span><span class="sxs-lookup"><span data-stu-id="e75c9-123">4</span></span>|<span data-ttu-id="e75c9-124">HTTP mit Internet peering gemischt</span><span class="sxs-lookup"><span data-stu-id="e75c9-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="e75c9-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="e75c9-125">simpleDownload</span></span>|<span data-ttu-id="e75c9-126">99</span><span class="sxs-lookup"><span data-stu-id="e75c9-126">99</span></span>|<span data-ttu-id="e75c9-127">Einfacher Downloadmodus mit keine peering</span><span class="sxs-lookup"><span data-stu-id="e75c9-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="e75c9-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="e75c9-128">bypassMode</span></span>|<span data-ttu-id="e75c9-129">100</span><span class="sxs-lookup"><span data-stu-id="e75c9-129">100</span></span>|<span data-ttu-id="e75c9-130">Umgehen Sie Modus.</span><span class="sxs-lookup"><span data-stu-id="e75c9-130">Bypass mode.</span></span> <span data-ttu-id="e75c9-131">Keine verwenden Sie Übermittlung Optimierung und verwenden Sie stattdessen BITS</span><span class="sxs-lookup"><span data-stu-id="e75c9-131">Do not use Delivery Optimization and use BITS instead</span></span>|



