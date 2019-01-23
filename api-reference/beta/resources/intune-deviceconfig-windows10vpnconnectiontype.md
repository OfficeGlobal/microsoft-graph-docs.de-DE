---
title: windows10VpnConnectionType Enum-Typ
description: VPN-Verbindungstypen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b3114c5d608cfed786fab8d2734d723682670ba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395937"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="97f70-103">windows10VpnConnectionType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="97f70-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="97f70-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="97f70-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="97f70-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97f70-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97f70-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="97f70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97f70-107">VPN-Verbindungstypen.</span><span class="sxs-lookup"><span data-stu-id="97f70-107">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="97f70-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="97f70-108">Members</span></span>
|<span data-ttu-id="97f70-109">Member</span><span class="sxs-lookup"><span data-stu-id="97f70-109">Member</span></span>|<span data-ttu-id="97f70-110">Wert</span><span class="sxs-lookup"><span data-stu-id="97f70-110">Value</span></span>|<span data-ttu-id="97f70-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97f70-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97f70-112">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="97f70-112">pulseSecure</span></span>|<span data-ttu-id="97f70-113">0</span><span class="sxs-lookup"><span data-stu-id="97f70-113">0</span></span>|<span data-ttu-id="97f70-114">Pulse sichern.</span><span class="sxs-lookup"><span data-stu-id="97f70-114">Pulse Secure.</span></span>|
|<span data-ttu-id="97f70-115">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="97f70-115">f5EdgeClient</span></span>|<span data-ttu-id="97f70-116">1</span><span class="sxs-lookup"><span data-stu-id="97f70-116">1</span></span>|<span data-ttu-id="97f70-117">F5-Edge-Client.</span><span class="sxs-lookup"><span data-stu-id="97f70-117">F5 Edge Client.</span></span>|
|<span data-ttu-id="97f70-118">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="97f70-118">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="97f70-119">2</span><span class="sxs-lookup"><span data-stu-id="97f70-119">2</span></span>|<span data-ttu-id="97f70-120">Dell SonicWALL Mobile Verbindung.</span><span class="sxs-lookup"><span data-stu-id="97f70-120">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="97f70-121">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="97f70-121">checkPointCapsuleVpn</span></span>|<span data-ttu-id="97f70-122">3</span><span class="sxs-lookup"><span data-stu-id="97f70-122">3</span></span>|<span data-ttu-id="97f70-123">Überprüfen Sie Punkt "Kapseln" VPN.</span><span class="sxs-lookup"><span data-stu-id="97f70-123">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="97f70-124">Automatisch</span><span class="sxs-lookup"><span data-stu-id="97f70-124">automatic</span></span>|<span data-ttu-id="97f70-125">4</span><span class="sxs-lookup"><span data-stu-id="97f70-125">4</span></span>|<span data-ttu-id="97f70-126">Automatisch.</span><span class="sxs-lookup"><span data-stu-id="97f70-126">Automatic.</span></span>|
|<span data-ttu-id="97f70-127">ikEv2</span><span class="sxs-lookup"><span data-stu-id="97f70-127">ikEv2</span></span>|<span data-ttu-id="97f70-128">5</span><span class="sxs-lookup"><span data-stu-id="97f70-128">5</span></span>|<span data-ttu-id="97f70-129">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="97f70-129">IKEv2.</span></span>|
|<span data-ttu-id="97f70-130">L2TP</span><span class="sxs-lookup"><span data-stu-id="97f70-130">l2tp</span></span>|<span data-ttu-id="97f70-131">6</span><span class="sxs-lookup"><span data-stu-id="97f70-131">6</span></span>|<span data-ttu-id="97f70-132">L2TP.</span><span class="sxs-lookup"><span data-stu-id="97f70-132">L2TP.</span></span>|
|<span data-ttu-id="97f70-133">PPTP</span><span class="sxs-lookup"><span data-stu-id="97f70-133">pptp</span></span>|<span data-ttu-id="97f70-134">7</span><span class="sxs-lookup"><span data-stu-id="97f70-134">7</span></span>|<span data-ttu-id="97f70-135">PPTP.</span><span class="sxs-lookup"><span data-stu-id="97f70-135">PPTP.</span></span>|
|<span data-ttu-id="97f70-136">Citrix</span><span class="sxs-lookup"><span data-stu-id="97f70-136">citrix</span></span>|<span data-ttu-id="97f70-137">8</span><span class="sxs-lookup"><span data-stu-id="97f70-137">8</span></span>|<span data-ttu-id="97f70-138">Citrix.</span><span class="sxs-lookup"><span data-stu-id="97f70-138">Citrix.</span></span>|
|<span data-ttu-id="97f70-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="97f70-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="97f70-140">9</span><span class="sxs-lookup"><span data-stu-id="97f70-140">9</span></span>|<span data-ttu-id="97f70-141">Palo Alto Netzwerke GlobalProtect.</span><span class="sxs-lookup"><span data-stu-id="97f70-141">Palo Alto Networks GlobalProtect.</span></span>|




