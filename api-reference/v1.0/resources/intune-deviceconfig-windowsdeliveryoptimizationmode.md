---
title: WindowsDeliveryOptimizationMode Enum-Typ
description: Übermittlung Optimierung Modus für Peer-Verteilung
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f80c6b5cbe7316c851954154bdb559f370f02b79
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951516"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="54aaa-103">WindowsDeliveryOptimizationMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="54aaa-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="54aaa-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="54aaa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54aaa-105">Übermittlung Optimierung Modus für Peer-Verteilung</span><span class="sxs-lookup"><span data-stu-id="54aaa-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="54aaa-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="54aaa-106">Members</span></span>
|<span data-ttu-id="54aaa-107">Element</span><span class="sxs-lookup"><span data-stu-id="54aaa-107">Member</span></span>|<span data-ttu-id="54aaa-108">Wert</span><span class="sxs-lookup"><span data-stu-id="54aaa-108">Value</span></span>|<span data-ttu-id="54aaa-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54aaa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54aaa-110">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="54aaa-110">userDefined</span></span>|<span data-ttu-id="54aaa-111">0</span><span class="sxs-lookup"><span data-stu-id="54aaa-111">0</span></span>|<span data-ttu-id="54aaa-112">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="54aaa-112">Allow the user to set.</span></span>|
|<span data-ttu-id="54aaa-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="54aaa-113">httpOnly</span></span>|<span data-ttu-id="54aaa-114">1</span><span class="sxs-lookup"><span data-stu-id="54aaa-114">1</span></span>|<span data-ttu-id="54aaa-115">Nur HTTP keine peering</span><span class="sxs-lookup"><span data-stu-id="54aaa-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="54aaa-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="54aaa-116">httpWithPeeringNat</span></span>|<span data-ttu-id="54aaa-117">2</span><span class="sxs-lookup"><span data-stu-id="54aaa-117">2</span></span>|<span data-ttu-id="54aaa-118">OS Standard – gemischt Http mit hinter den gleichen Network Address Translation peering</span><span class="sxs-lookup"><span data-stu-id="54aaa-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="54aaa-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="54aaa-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="54aaa-120">3</span><span class="sxs-lookup"><span data-stu-id="54aaa-120">3</span></span>|<span data-ttu-id="54aaa-121">HTTP mit über eine private Gruppe peering gemischt</span><span class="sxs-lookup"><span data-stu-id="54aaa-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="54aaa-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="54aaa-122">httpWithInternetPeering</span></span>|<span data-ttu-id="54aaa-123">4</span><span class="sxs-lookup"><span data-stu-id="54aaa-123">4</span></span>|<span data-ttu-id="54aaa-124">HTTP mit Internet peering gemischt</span><span class="sxs-lookup"><span data-stu-id="54aaa-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="54aaa-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="54aaa-125">simpleDownload</span></span>|<span data-ttu-id="54aaa-126">99</span><span class="sxs-lookup"><span data-stu-id="54aaa-126">99</span></span>|<span data-ttu-id="54aaa-127">Einfacher Downloadmodus mit keine peering</span><span class="sxs-lookup"><span data-stu-id="54aaa-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="54aaa-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="54aaa-128">bypassMode</span></span>|<span data-ttu-id="54aaa-129">100</span><span class="sxs-lookup"><span data-stu-id="54aaa-129">100</span></span>|<span data-ttu-id="54aaa-130">Umgehen Sie Modus.</span><span class="sxs-lookup"><span data-stu-id="54aaa-130">Bypass mode.</span></span> <span data-ttu-id="54aaa-131">Keine verwenden Sie Übermittlung Optimierung und verwenden Sie stattdessen BITS</span><span class="sxs-lookup"><span data-stu-id="54aaa-131">Do not use Delivery Optimization and use BITS instead</span></span>|



