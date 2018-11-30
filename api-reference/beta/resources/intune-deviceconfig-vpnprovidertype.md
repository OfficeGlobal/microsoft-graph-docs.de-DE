---
title: VpnProviderType Enum-Typ
description: Providertyp für VPN-app.
ms.openlocfilehash: 133b1663ce3c72ba520dd5c1eeadf963154e9cc9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064326"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="b05ab-103">VpnProviderType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="b05ab-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="b05ab-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b05ab-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b05ab-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b05ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b05ab-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b05ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b05ab-107">Providertyp für VPN-app.</span><span class="sxs-lookup"><span data-stu-id="b05ab-107">Provider type for per-app VPN.</span></span>
## <a name="members"></a><span data-ttu-id="b05ab-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="b05ab-108">Members</span></span>
|<span data-ttu-id="b05ab-109">Element</span><span class="sxs-lookup"><span data-stu-id="b05ab-109">Member</span></span>|<span data-ttu-id="b05ab-110">Wert</span><span class="sxs-lookup"><span data-stu-id="b05ab-110">Value</span></span>|<span data-ttu-id="b05ab-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b05ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b05ab-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="b05ab-112">notConfigured</span></span>|<span data-ttu-id="b05ab-113">0</span><span class="sxs-lookup"><span data-stu-id="b05ab-113">0</span></span>|<span data-ttu-id="b05ab-114">Für den Tunnel wird nicht explizit konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="b05ab-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="b05ab-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="b05ab-115">appProxy</span></span>|<span data-ttu-id="b05ab-116">1</span><span class="sxs-lookup"><span data-stu-id="b05ab-116">1</span></span>|<span data-ttu-id="b05ab-117">Tunnel Datenverkehr auf Anwendungsebene.</span><span class="sxs-lookup"><span data-stu-id="b05ab-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="b05ab-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="b05ab-118">packetTunnel</span></span>|<span data-ttu-id="b05ab-119">2</span><span class="sxs-lookup"><span data-stu-id="b05ab-119">2</span></span>|<span data-ttu-id="b05ab-120">Der IP-Ebene für den Tunnel.</span><span class="sxs-lookup"><span data-stu-id="b05ab-120">Tunnel traffic at the IP layer.</span></span>|





