---
title: VpnProviderType Enum-Typ
description: Providertyp für VPN-app.
author: tfitzmac
ms.openlocfilehash: d8f002582879302bcbe0fb965110eaa5e674a689
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351597"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="73a1a-103">VpnProviderType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="73a1a-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="73a1a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="73a1a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73a1a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="73a1a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73a1a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="73a1a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73a1a-107">Providertyp für VPN-app.</span><span class="sxs-lookup"><span data-stu-id="73a1a-107">Provider type for per-app VPN.</span></span>
## <a name="members"></a><span data-ttu-id="73a1a-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="73a1a-108">Members</span></span>
|<span data-ttu-id="73a1a-109">Member</span><span class="sxs-lookup"><span data-stu-id="73a1a-109">Member</span></span>|<span data-ttu-id="73a1a-110">Wert</span><span class="sxs-lookup"><span data-stu-id="73a1a-110">Value</span></span>|<span data-ttu-id="73a1a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73a1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73a1a-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="73a1a-112">notConfigured</span></span>|<span data-ttu-id="73a1a-113">0</span><span class="sxs-lookup"><span data-stu-id="73a1a-113">0</span></span>|<span data-ttu-id="73a1a-114">Für den Tunnel wird nicht explizit konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="73a1a-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="73a1a-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="73a1a-115">appProxy</span></span>|<span data-ttu-id="73a1a-116">1</span><span class="sxs-lookup"><span data-stu-id="73a1a-116">1</span></span>|<span data-ttu-id="73a1a-117">Tunnel Datenverkehr auf Anwendungsebene.</span><span class="sxs-lookup"><span data-stu-id="73a1a-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="73a1a-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="73a1a-118">packetTunnel</span></span>|<span data-ttu-id="73a1a-119">2</span><span class="sxs-lookup"><span data-stu-id="73a1a-119">2</span></span>|<span data-ttu-id="73a1a-120">Der IP-Ebene für den Tunnel.</span><span class="sxs-lookup"><span data-stu-id="73a1a-120">Tunnel traffic at the IP layer.</span></span>|





