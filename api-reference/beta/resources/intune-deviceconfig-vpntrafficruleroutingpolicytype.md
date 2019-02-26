---
title: vpnTrafficRuleRoutingPolicyType-Enumerationstyp
description: Gibt die Routing Richtlinie für eine VPN-Datenverkehrs Regel an.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a7c6121b9adc47d116a7b3321ca150a8d42449a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157344"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="0ca14-103">vpnTrafficRuleRoutingPolicyType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="0ca14-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="0ca14-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0ca14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ca14-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0ca14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ca14-106">Gibt die Routing Richtlinie für eine VPN-Datenverkehrs Regel an.</span><span class="sxs-lookup"><span data-stu-id="0ca14-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="0ca14-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="0ca14-107">Members</span></span>
|<span data-ttu-id="0ca14-108">Element</span><span class="sxs-lookup"><span data-stu-id="0ca14-108">Member</span></span>|<span data-ttu-id="0ca14-109">Wert</span><span class="sxs-lookup"><span data-stu-id="0ca14-109">Value</span></span>|<span data-ttu-id="0ca14-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0ca14-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ca14-111">Keine</span><span class="sxs-lookup"><span data-stu-id="0ca14-111">none</span></span>|<span data-ttu-id="0ca14-112">0</span><span class="sxs-lookup"><span data-stu-id="0ca14-112">0</span></span>|<span data-ttu-id="0ca14-113">Es wurde keine Routing Richtlinie angegeben.</span><span class="sxs-lookup"><span data-stu-id="0ca14-113">No routing policy specified.</span></span>|
|<span data-ttu-id="0ca14-114">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="0ca14-114">splitTunnel</span></span>|<span data-ttu-id="0ca14-115">1</span><span class="sxs-lookup"><span data-stu-id="0ca14-115">1</span></span>|<span data-ttu-id="0ca14-116">Der Netzwerkdatenverkehr für die angegebene APP wird über das VPN weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="0ca14-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="0ca14-117">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="0ca14-117">forceTunnel</span></span>|<span data-ttu-id="0ca14-118">2</span><span class="sxs-lookup"><span data-stu-id="0ca14-118">2</span></span>|<span data-ttu-id="0ca14-119">Der gesamte Netzwerkdatenverkehr wird über das VPN weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="0ca14-119">All network traffic will be routed through the VPN.</span></span>|




