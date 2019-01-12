---
title: VpnProviderType Enum-Typ
description: Providertyp für VPN-app.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1eeb0acf2f6e7b0773cbf4697e5a27699d1f2f27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937726"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="3b039-103">VpnProviderType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="3b039-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="3b039-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3b039-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b039-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b039-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b039-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3b039-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b039-107">Providertyp für VPN-app.</span><span class="sxs-lookup"><span data-stu-id="3b039-107">Provider type for per-app VPN.</span></span>
## <a name="members"></a><span data-ttu-id="3b039-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="3b039-108">Members</span></span>
|<span data-ttu-id="3b039-109">Element</span><span class="sxs-lookup"><span data-stu-id="3b039-109">Member</span></span>|<span data-ttu-id="3b039-110">Wert</span><span class="sxs-lookup"><span data-stu-id="3b039-110">Value</span></span>|<span data-ttu-id="3b039-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b039-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b039-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="3b039-112">notConfigured</span></span>|<span data-ttu-id="3b039-113">0</span><span class="sxs-lookup"><span data-stu-id="3b039-113">0</span></span>|<span data-ttu-id="3b039-114">Für den Tunnel wird nicht explizit konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="3b039-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="3b039-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="3b039-115">appProxy</span></span>|<span data-ttu-id="3b039-116">1</span><span class="sxs-lookup"><span data-stu-id="3b039-116">1</span></span>|<span data-ttu-id="3b039-117">Tunnel Datenverkehr auf Anwendungsebene.</span><span class="sxs-lookup"><span data-stu-id="3b039-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="3b039-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="3b039-118">packetTunnel</span></span>|<span data-ttu-id="3b039-119">2</span><span class="sxs-lookup"><span data-stu-id="3b039-119">2</span></span>|<span data-ttu-id="3b039-120">Der IP-Ebene für den Tunnel.</span><span class="sxs-lookup"><span data-stu-id="3b039-120">Tunnel traffic at the IP layer.</span></span>|





