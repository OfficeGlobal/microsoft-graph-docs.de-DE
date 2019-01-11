---
title: VpnProviderType Enum-Typ
description: Providertyp für VPN-app.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ea3e3fcac5fc84270fcdb63b6ab673cb9f55aea9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861285"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="84730-103">VpnProviderType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="84730-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="84730-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="84730-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84730-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="84730-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84730-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="84730-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84730-107">Providertyp für VPN-app.</span><span class="sxs-lookup"><span data-stu-id="84730-107">Provider type for per-app VPN.</span></span>
## <a name="members"></a><span data-ttu-id="84730-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="84730-108">Members</span></span>
|<span data-ttu-id="84730-109">Element</span><span class="sxs-lookup"><span data-stu-id="84730-109">Member</span></span>|<span data-ttu-id="84730-110">Wert</span><span class="sxs-lookup"><span data-stu-id="84730-110">Value</span></span>|<span data-ttu-id="84730-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84730-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84730-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="84730-112">notConfigured</span></span>|<span data-ttu-id="84730-113">0</span><span class="sxs-lookup"><span data-stu-id="84730-113">0</span></span>|<span data-ttu-id="84730-114">Für den Tunnel wird nicht explizit konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="84730-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="84730-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="84730-115">appProxy</span></span>|<span data-ttu-id="84730-116">1</span><span class="sxs-lookup"><span data-stu-id="84730-116">1</span></span>|<span data-ttu-id="84730-117">Tunnel Datenverkehr auf Anwendungsebene.</span><span class="sxs-lookup"><span data-stu-id="84730-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="84730-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="84730-118">packetTunnel</span></span>|<span data-ttu-id="84730-119">2</span><span class="sxs-lookup"><span data-stu-id="84730-119">2</span></span>|<span data-ttu-id="84730-120">Der IP-Ebene für den Tunnel.</span><span class="sxs-lookup"><span data-stu-id="84730-120">Tunnel traffic at the IP layer.</span></span>|





