---
title: VpnTrafficRuleRoutingPolicyType Enum-Typ
description: Gibt die routing-Richtlinie für eine VPN-Datenverkehr Regel an.
author: tfitzmac
ms.openlocfilehash: 5aa3f44f0e4ccf177154f97e9849093c52728b2e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343421"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="d801b-103">VpnTrafficRuleRoutingPolicyType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="d801b-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="d801b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d801b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d801b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d801b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d801b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d801b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d801b-107">Gibt die routing-Richtlinie für eine VPN-Datenverkehr Regel an.</span><span class="sxs-lookup"><span data-stu-id="d801b-107">Specifies the routing policy for a VPN traffic rule.</span></span>
## <a name="members"></a><span data-ttu-id="d801b-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="d801b-108">Members</span></span>
|<span data-ttu-id="d801b-109">Member</span><span class="sxs-lookup"><span data-stu-id="d801b-109">Member</span></span>|<span data-ttu-id="d801b-110">Wert</span><span class="sxs-lookup"><span data-stu-id="d801b-110">Value</span></span>|<span data-ttu-id="d801b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d801b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d801b-112">Keine</span><span class="sxs-lookup"><span data-stu-id="d801b-112">none</span></span>|<span data-ttu-id="d801b-113">0</span><span class="sxs-lookup"><span data-stu-id="d801b-113">0</span></span>|<span data-ttu-id="d801b-114">Kein routing-Richtlinie angegeben.</span><span class="sxs-lookup"><span data-stu-id="d801b-114">No routing policy specified.</span></span>|
|<span data-ttu-id="d801b-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="d801b-115">splitTunnel</span></span>|<span data-ttu-id="d801b-116">1</span><span class="sxs-lookup"><span data-stu-id="d801b-116">1</span></span>|<span data-ttu-id="d801b-117">Netzwerkverkehr für das angegebene app werden über VPN weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="d801b-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="d801b-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="d801b-118">forceTunnel</span></span>|<span data-ttu-id="d801b-119">2</span><span class="sxs-lookup"><span data-stu-id="d801b-119">2</span></span>|<span data-ttu-id="d801b-120">Durch das VPN werden alle Netzwerkdatenverkehr weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="d801b-120">All network traffic will be routed through the VPN.</span></span>|





