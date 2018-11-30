---
title: VpnTrafficRuleRoutingPolicyType Enum-Typ
description: Gibt die routing-Richtlinie für eine VPN-Datenverkehr Regel an.
ms.openlocfilehash: df51851ef0820f5982a6689421503364e9064c78
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060904"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="a7f41-103">VpnTrafficRuleRoutingPolicyType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="a7f41-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="a7f41-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a7f41-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7f41-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a7f41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7f41-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a7f41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7f41-107">Gibt die routing-Richtlinie für eine VPN-Datenverkehr Regel an.</span><span class="sxs-lookup"><span data-stu-id="a7f41-107">Specifies the routing policy for a VPN traffic rule.</span></span>
## <a name="members"></a><span data-ttu-id="a7f41-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="a7f41-108">Members</span></span>
|<span data-ttu-id="a7f41-109">Element</span><span class="sxs-lookup"><span data-stu-id="a7f41-109">Member</span></span>|<span data-ttu-id="a7f41-110">Wert</span><span class="sxs-lookup"><span data-stu-id="a7f41-110">Value</span></span>|<span data-ttu-id="a7f41-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a7f41-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7f41-112">n/v</span><span class="sxs-lookup"><span data-stu-id="a7f41-112">none</span></span>|<span data-ttu-id="a7f41-113">0</span><span class="sxs-lookup"><span data-stu-id="a7f41-113">0</span></span>|<span data-ttu-id="a7f41-114">Kein routing-Richtlinie angegeben.</span><span class="sxs-lookup"><span data-stu-id="a7f41-114">No routing policy specified.</span></span>|
|<span data-ttu-id="a7f41-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="a7f41-115">splitTunnel</span></span>|<span data-ttu-id="a7f41-116">1</span><span class="sxs-lookup"><span data-stu-id="a7f41-116">1</span></span>|<span data-ttu-id="a7f41-117">Netzwerkverkehr für das angegebene app werden über VPN weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="a7f41-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="a7f41-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="a7f41-118">forceTunnel</span></span>|<span data-ttu-id="a7f41-119">2</span><span class="sxs-lookup"><span data-stu-id="a7f41-119">2</span></span>|<span data-ttu-id="a7f41-120">Durch das VPN werden alle Netzwerkdatenverkehr weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="a7f41-120">All network traffic will be routed through the VPN.</span></span>|





