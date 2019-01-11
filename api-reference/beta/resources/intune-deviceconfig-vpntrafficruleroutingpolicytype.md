---
title: VpnTrafficRuleRoutingPolicyType Enum-Typ
description: Gibt die routing-Richtlinie für eine VPN-Datenverkehr Regel an.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2b44a2b58cc42e9f3f88964d79473327f4ca2b74
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855321"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="bdb31-103">VpnTrafficRuleRoutingPolicyType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="bdb31-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="bdb31-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bdb31-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdb31-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bdb31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bdb31-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bdb31-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdb31-107">Gibt die routing-Richtlinie für eine VPN-Datenverkehr Regel an.</span><span class="sxs-lookup"><span data-stu-id="bdb31-107">Specifies the routing policy for a VPN traffic rule.</span></span>
## <a name="members"></a><span data-ttu-id="bdb31-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="bdb31-108">Members</span></span>
|<span data-ttu-id="bdb31-109">Element</span><span class="sxs-lookup"><span data-stu-id="bdb31-109">Member</span></span>|<span data-ttu-id="bdb31-110">Wert</span><span class="sxs-lookup"><span data-stu-id="bdb31-110">Value</span></span>|<span data-ttu-id="bdb31-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bdb31-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdb31-112">n/v</span><span class="sxs-lookup"><span data-stu-id="bdb31-112">none</span></span>|<span data-ttu-id="bdb31-113">0</span><span class="sxs-lookup"><span data-stu-id="bdb31-113">0</span></span>|<span data-ttu-id="bdb31-114">Kein routing-Richtlinie angegeben.</span><span class="sxs-lookup"><span data-stu-id="bdb31-114">No routing policy specified.</span></span>|
|<span data-ttu-id="bdb31-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="bdb31-115">splitTunnel</span></span>|<span data-ttu-id="bdb31-116">1</span><span class="sxs-lookup"><span data-stu-id="bdb31-116">1</span></span>|<span data-ttu-id="bdb31-117">Netzwerkverkehr für das angegebene app werden über VPN weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="bdb31-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="bdb31-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="bdb31-118">forceTunnel</span></span>|<span data-ttu-id="bdb31-119">2</span><span class="sxs-lookup"><span data-stu-id="bdb31-119">2</span></span>|<span data-ttu-id="bdb31-120">Durch das VPN werden alle Netzwerkdatenverkehr weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="bdb31-120">All network traffic will be routed through the VPN.</span></span>|





