---
title: WindowsDeliveryOptimizationMode Enum-Typ
description: Übermittlung Optimierung Modus für Peer-Verteilung
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5565965f9ba9395d7cd07b2935e6772478e0bb50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406885"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="df19b-103">WindowsDeliveryOptimizationMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="df19b-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="df19b-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="df19b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="df19b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df19b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df19b-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="df19b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df19b-107">Übermittlung Optimierung Modus für Peer-Verteilung</span><span class="sxs-lookup"><span data-stu-id="df19b-107">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="df19b-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="df19b-108">Members</span></span>
|<span data-ttu-id="df19b-109">Member</span><span class="sxs-lookup"><span data-stu-id="df19b-109">Member</span></span>|<span data-ttu-id="df19b-110">Wert</span><span class="sxs-lookup"><span data-stu-id="df19b-110">Value</span></span>|<span data-ttu-id="df19b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df19b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df19b-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="df19b-112">userDefined</span></span>|<span data-ttu-id="df19b-113">0</span><span class="sxs-lookup"><span data-stu-id="df19b-113">0</span></span>|<span data-ttu-id="df19b-114">Ermöglicht es dem Benutzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="df19b-114">Allow the user to set.</span></span>|
|<span data-ttu-id="df19b-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="df19b-115">httpOnly</span></span>|<span data-ttu-id="df19b-116">1</span><span class="sxs-lookup"><span data-stu-id="df19b-116">1</span></span>|<span data-ttu-id="df19b-117">Nur HTTP keine peering</span><span class="sxs-lookup"><span data-stu-id="df19b-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="df19b-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="df19b-118">httpWithPeeringNat</span></span>|<span data-ttu-id="df19b-119">2</span><span class="sxs-lookup"><span data-stu-id="df19b-119">2</span></span>|<span data-ttu-id="df19b-120">OS Standard – gemischt Http mit hinter den gleichen Network Address Translation peering</span><span class="sxs-lookup"><span data-stu-id="df19b-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="df19b-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="df19b-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="df19b-122">3</span><span class="sxs-lookup"><span data-stu-id="df19b-122">3</span></span>|<span data-ttu-id="df19b-123">HTTP mit über eine private Gruppe peering gemischt</span><span class="sxs-lookup"><span data-stu-id="df19b-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="df19b-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="df19b-124">httpWithInternetPeering</span></span>|<span data-ttu-id="df19b-125">4</span><span class="sxs-lookup"><span data-stu-id="df19b-125">4</span></span>|<span data-ttu-id="df19b-126">HTTP mit Internet peering gemischt</span><span class="sxs-lookup"><span data-stu-id="df19b-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="df19b-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="df19b-127">simpleDownload</span></span>|<span data-ttu-id="df19b-128">99</span><span class="sxs-lookup"><span data-stu-id="df19b-128">99</span></span>|<span data-ttu-id="df19b-129">Einfacher Downloadmodus mit keine peering</span><span class="sxs-lookup"><span data-stu-id="df19b-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="df19b-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="df19b-130">bypassMode</span></span>|<span data-ttu-id="df19b-131">100</span><span class="sxs-lookup"><span data-stu-id="df19b-131">100</span></span>|<span data-ttu-id="df19b-132">Umgehen Sie Modus.</span><span class="sxs-lookup"><span data-stu-id="df19b-132">Bypass mode.</span></span> <span data-ttu-id="df19b-133">Keine verwenden Sie Übermittlung Optimierung und verwenden Sie stattdessen BITS</span><span class="sxs-lookup"><span data-stu-id="df19b-133">Do not use Delivery Optimization and use BITS instead</span></span>|




