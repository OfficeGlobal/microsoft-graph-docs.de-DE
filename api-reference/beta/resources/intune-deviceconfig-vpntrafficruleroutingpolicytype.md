---
title: VpnTrafficRuleRoutingPolicyType Enum-Typ
description: Gibt die routing-Richtlinie für eine VPN-Datenverkehr Regel an.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 028e49085e4a1fa5f01ac59ff00fbafd8846dfb9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415005"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="9efb9-103">VpnTrafficRuleRoutingPolicyType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="9efb9-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="9efb9-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9efb9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9efb9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9efb9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9efb9-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9efb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9efb9-107">Gibt die routing-Richtlinie für eine VPN-Datenverkehr Regel an.</span><span class="sxs-lookup"><span data-stu-id="9efb9-107">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="9efb9-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="9efb9-108">Members</span></span>
|<span data-ttu-id="9efb9-109">Member</span><span class="sxs-lookup"><span data-stu-id="9efb9-109">Member</span></span>|<span data-ttu-id="9efb9-110">Wert</span><span class="sxs-lookup"><span data-stu-id="9efb9-110">Value</span></span>|<span data-ttu-id="9efb9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9efb9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9efb9-112">Keine</span><span class="sxs-lookup"><span data-stu-id="9efb9-112">none</span></span>|<span data-ttu-id="9efb9-113">0</span><span class="sxs-lookup"><span data-stu-id="9efb9-113">0</span></span>|<span data-ttu-id="9efb9-114">Kein routing-Richtlinie angegeben.</span><span class="sxs-lookup"><span data-stu-id="9efb9-114">No routing policy specified.</span></span>|
|<span data-ttu-id="9efb9-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="9efb9-115">splitTunnel</span></span>|<span data-ttu-id="9efb9-116">1</span><span class="sxs-lookup"><span data-stu-id="9efb9-116">1</span></span>|<span data-ttu-id="9efb9-117">Netzwerkverkehr für das angegebene app werden über VPN weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="9efb9-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="9efb9-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="9efb9-118">forceTunnel</span></span>|<span data-ttu-id="9efb9-119">2</span><span class="sxs-lookup"><span data-stu-id="9efb9-119">2</span></span>|<span data-ttu-id="9efb9-120">Durch das VPN werden alle Netzwerkdatenverkehr weitergeleitet.</span><span class="sxs-lookup"><span data-stu-id="9efb9-120">All network traffic will be routed through the VPN.</span></span>|




