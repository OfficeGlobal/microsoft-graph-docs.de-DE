---
title: AppleVpnConnectionType Enum-Typ
description: Typ des Apple VPN-Verbindung.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 94b39d6804a304cf84e6dbefa3ef715f837b55af
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912694"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="8b380-103">AppleVpnConnectionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="8b380-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="8b380-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8b380-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b380-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8b380-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b380-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8b380-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b380-107">Typ des Apple VPN-Verbindung.</span><span class="sxs-lookup"><span data-stu-id="8b380-107">Apple VPN connection type.</span></span>
## <a name="members"></a><span data-ttu-id="8b380-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="8b380-108">Members</span></span>
|<span data-ttu-id="8b380-109">Element</span><span class="sxs-lookup"><span data-stu-id="8b380-109">Member</span></span>|<span data-ttu-id="8b380-110">Wert</span><span class="sxs-lookup"><span data-stu-id="8b380-110">Value</span></span>|<span data-ttu-id="8b380-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b380-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b380-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="8b380-112">ciscoAnyConnect</span></span>|<span data-ttu-id="8b380-113">0</span><span class="sxs-lookup"><span data-stu-id="8b380-113">0</span></span>|<span data-ttu-id="8b380-114">Cisco AnyConnect.</span><span class="sxs-lookup"><span data-stu-id="8b380-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="8b380-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="8b380-115">pulseSecure</span></span>|<span data-ttu-id="8b380-116">1</span><span class="sxs-lookup"><span data-stu-id="8b380-116">1</span></span>|<span data-ttu-id="8b380-117">Pulse sichern.</span><span class="sxs-lookup"><span data-stu-id="8b380-117">Pulse Secure.</span></span>|
|<span data-ttu-id="8b380-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="8b380-118">f5EdgeClient</span></span>|<span data-ttu-id="8b380-119">2</span><span class="sxs-lookup"><span data-stu-id="8b380-119">2</span></span>|<span data-ttu-id="8b380-120">F5-Edge-Client.</span><span class="sxs-lookup"><span data-stu-id="8b380-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="8b380-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="8b380-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="8b380-122">3</span><span class="sxs-lookup"><span data-stu-id="8b380-122">3</span></span>|<span data-ttu-id="8b380-123">Dell SonicWALL Mobile Verbindung.</span><span class="sxs-lookup"><span data-stu-id="8b380-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="8b380-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="8b380-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="8b380-125">4</span><span class="sxs-lookup"><span data-stu-id="8b380-125">4</span></span>|<span data-ttu-id="8b380-126">Überprüfen Sie Punkt "Kapseln" VPN.</span><span class="sxs-lookup"><span data-stu-id="8b380-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="8b380-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="8b380-127">customVpn</span></span>|<span data-ttu-id="8b380-128">5</span><span class="sxs-lookup"><span data-stu-id="8b380-128">5</span></span>|<span data-ttu-id="8b380-129">Benutzerdefinierte VPN.</span><span class="sxs-lookup"><span data-stu-id="8b380-129">Custom VPN.</span></span>|
|<span data-ttu-id="8b380-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="8b380-130">ciscoIPSec</span></span>|<span data-ttu-id="8b380-131">6</span><span class="sxs-lookup"><span data-stu-id="8b380-131">6</span></span>|<span data-ttu-id="8b380-132">Cisco (IPSec).</span><span class="sxs-lookup"><span data-stu-id="8b380-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="8b380-133">Citrix</span><span class="sxs-lookup"><span data-stu-id="8b380-133">citrix</span></span>|<span data-ttu-id="8b380-134">7</span><span class="sxs-lookup"><span data-stu-id="8b380-134">7</span></span>|<span data-ttu-id="8b380-135">Citrix.</span><span class="sxs-lookup"><span data-stu-id="8b380-135">Citrix.</span></span>|
|<span data-ttu-id="8b380-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="8b380-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="8b380-137">8</span><span class="sxs-lookup"><span data-stu-id="8b380-137">8</span></span>|<span data-ttu-id="8b380-138">Cisco AnyConnect V2.</span><span class="sxs-lookup"><span data-stu-id="8b380-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="8b380-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="8b380-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="8b380-140">9</span><span class="sxs-lookup"><span data-stu-id="8b380-140">9</span></span>|<span data-ttu-id="8b380-141">Palo Alto Netzwerke GlobalProtect.</span><span class="sxs-lookup"><span data-stu-id="8b380-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="8b380-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="8b380-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="8b380-143">10</span><span class="sxs-lookup"><span data-stu-id="8b380-143">10</span></span>|<span data-ttu-id="8b380-144">Zscaler privater Zugriff.</span><span class="sxs-lookup"><span data-stu-id="8b380-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="8b380-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="8b380-145">f5Access2018</span></span>|<span data-ttu-id="8b380-146">11</span><span class="sxs-lookup"><span data-stu-id="8b380-146">11</span></span>|<span data-ttu-id="8b380-147">F5 Access 2018.</span><span class="sxs-lookup"><span data-stu-id="8b380-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="8b380-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="8b380-148">citrixSso</span></span>|<span data-ttu-id="8b380-149">12</span><span class="sxs-lookup"><span data-stu-id="8b380-149">12</span></span>|<span data-ttu-id="8b380-150">Citrix Sso.</span><span class="sxs-lookup"><span data-stu-id="8b380-150">Citrix Sso.</span></span>|
|<span data-ttu-id="8b380-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="8b380-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="8b380-152">13</span><span class="sxs-lookup"><span data-stu-id="8b380-152">13</span></span>|<span data-ttu-id="8b380-153">Palo auch Netzwerke GlobalProtect V2.</span><span class="sxs-lookup"><span data-stu-id="8b380-153">Palo Alto Networks GlobalProtect V2.</span></span>|





