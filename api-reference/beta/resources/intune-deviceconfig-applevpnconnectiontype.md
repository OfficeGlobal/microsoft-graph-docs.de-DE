---
title: AppleVpnConnectionType Enum-Typ
description: Typ des Apple VPN-Verbindung.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 46469b21fecdec5f4a7bb97d09eed9c9345914b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842161"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="146bb-103">AppleVpnConnectionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="146bb-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="146bb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="146bb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="146bb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="146bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="146bb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="146bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="146bb-107">Typ des Apple VPN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="146bb-107">Apple VPN connection type.</span></span>
## <a name="members"></a><span data-ttu-id="146bb-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="146bb-108">Members</span></span>
|<span data-ttu-id="146bb-109">Element</span><span class="sxs-lookup"><span data-stu-id="146bb-109">Member</span></span>|<span data-ttu-id="146bb-110">Wert</span><span class="sxs-lookup"><span data-stu-id="146bb-110">Value</span></span>|<span data-ttu-id="146bb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="146bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="146bb-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="146bb-112">ciscoAnyConnect</span></span>|<span data-ttu-id="146bb-113">0</span><span class="sxs-lookup"><span data-stu-id="146bb-113">0</span></span>|<span data-ttu-id="146bb-114">Cisco AnyConnect.</span><span class="sxs-lookup"><span data-stu-id="146bb-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="146bb-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="146bb-115">pulseSecure</span></span>|<span data-ttu-id="146bb-116">1</span><span class="sxs-lookup"><span data-stu-id="146bb-116">1</span></span>|<span data-ttu-id="146bb-117">Pulse sichern.</span><span class="sxs-lookup"><span data-stu-id="146bb-117">Pulse Secure.</span></span>|
|<span data-ttu-id="146bb-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="146bb-118">f5EdgeClient</span></span>|<span data-ttu-id="146bb-119">2</span><span class="sxs-lookup"><span data-stu-id="146bb-119">2</span></span>|<span data-ttu-id="146bb-120">F5-Edge-Client.</span><span class="sxs-lookup"><span data-stu-id="146bb-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="146bb-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="146bb-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="146bb-122">3</span><span class="sxs-lookup"><span data-stu-id="146bb-122">3</span></span>|<span data-ttu-id="146bb-123">Dell SonicWALL Mobile Verbindung.</span><span class="sxs-lookup"><span data-stu-id="146bb-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="146bb-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="146bb-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="146bb-125">4</span><span class="sxs-lookup"><span data-stu-id="146bb-125">4</span></span>|<span data-ttu-id="146bb-126">Überprüfen Sie Punkt "Kapseln" VPN.</span><span class="sxs-lookup"><span data-stu-id="146bb-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="146bb-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="146bb-127">customVpn</span></span>|<span data-ttu-id="146bb-128">5</span><span class="sxs-lookup"><span data-stu-id="146bb-128">5</span></span>|<span data-ttu-id="146bb-129">Benutzerdefinierte VPN.</span><span class="sxs-lookup"><span data-stu-id="146bb-129">Custom VPN.</span></span>|
|<span data-ttu-id="146bb-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="146bb-130">ciscoIPSec</span></span>|<span data-ttu-id="146bb-131">6</span><span class="sxs-lookup"><span data-stu-id="146bb-131">6</span></span>|<span data-ttu-id="146bb-132">Cisco (IPSec).</span><span class="sxs-lookup"><span data-stu-id="146bb-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="146bb-133">Citrix</span><span class="sxs-lookup"><span data-stu-id="146bb-133">citrix</span></span>|<span data-ttu-id="146bb-134">7</span><span class="sxs-lookup"><span data-stu-id="146bb-134">7</span></span>|<span data-ttu-id="146bb-135">Citrix.</span><span class="sxs-lookup"><span data-stu-id="146bb-135">Citrix.</span></span>|
|<span data-ttu-id="146bb-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="146bb-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="146bb-137">8</span><span class="sxs-lookup"><span data-stu-id="146bb-137">8</span></span>|<span data-ttu-id="146bb-138">Cisco AnyConnect V2.</span><span class="sxs-lookup"><span data-stu-id="146bb-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="146bb-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="146bb-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="146bb-140">9</span><span class="sxs-lookup"><span data-stu-id="146bb-140">9</span></span>|<span data-ttu-id="146bb-141">Palo Alto Netzwerke GlobalProtect.</span><span class="sxs-lookup"><span data-stu-id="146bb-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="146bb-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="146bb-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="146bb-143">10</span><span class="sxs-lookup"><span data-stu-id="146bb-143">10</span></span>|<span data-ttu-id="146bb-144">Zscaler privater Zugriff.</span><span class="sxs-lookup"><span data-stu-id="146bb-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="146bb-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="146bb-145">f5Access2018</span></span>|<span data-ttu-id="146bb-146">11</span><span class="sxs-lookup"><span data-stu-id="146bb-146">11</span></span>|<span data-ttu-id="146bb-147">F5 Access 2018.</span><span class="sxs-lookup"><span data-stu-id="146bb-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="146bb-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="146bb-148">citrixSso</span></span>|<span data-ttu-id="146bb-149">12</span><span class="sxs-lookup"><span data-stu-id="146bb-149">12</span></span>|<span data-ttu-id="146bb-150">Citrix Sso.</span><span class="sxs-lookup"><span data-stu-id="146bb-150">Citrix Sso.</span></span>|
|<span data-ttu-id="146bb-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="146bb-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="146bb-152">13</span><span class="sxs-lookup"><span data-stu-id="146bb-152">13</span></span>|<span data-ttu-id="146bb-153">Palo auch Netzwerke GlobalProtect V2.</span><span class="sxs-lookup"><span data-stu-id="146bb-153">Palo Alto Networks GlobalProtect V2.</span></span>|





