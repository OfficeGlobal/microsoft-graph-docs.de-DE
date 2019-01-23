---
title: VpnProviderType Enum-Typ
description: Providertyp für VPN-app.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2de8f78222ba0c945000b84f28039c2f6af58daa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407221"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="0c2a4-103">VpnProviderType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="0c2a4-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="0c2a4-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0c2a4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0c2a4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0c2a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c2a4-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0c2a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c2a4-107">Providertyp für VPN-app.</span><span class="sxs-lookup"><span data-stu-id="0c2a4-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="0c2a4-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="0c2a4-108">Members</span></span>
|<span data-ttu-id="0c2a4-109">Member</span><span class="sxs-lookup"><span data-stu-id="0c2a4-109">Member</span></span>|<span data-ttu-id="0c2a4-110">Wert</span><span class="sxs-lookup"><span data-stu-id="0c2a4-110">Value</span></span>|<span data-ttu-id="0c2a4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c2a4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c2a4-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="0c2a4-112">notConfigured</span></span>|<span data-ttu-id="0c2a4-113">0</span><span class="sxs-lookup"><span data-stu-id="0c2a4-113">0</span></span>|<span data-ttu-id="0c2a4-114">Für den Tunnel wird nicht explizit konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="0c2a4-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="0c2a4-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="0c2a4-115">appProxy</span></span>|<span data-ttu-id="0c2a4-116">1</span><span class="sxs-lookup"><span data-stu-id="0c2a4-116">1</span></span>|<span data-ttu-id="0c2a4-117">Tunnel Datenverkehr auf Anwendungsebene.</span><span class="sxs-lookup"><span data-stu-id="0c2a4-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="0c2a4-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="0c2a4-118">packetTunnel</span></span>|<span data-ttu-id="0c2a4-119">2</span><span class="sxs-lookup"><span data-stu-id="0c2a4-119">2</span></span>|<span data-ttu-id="0c2a4-120">Der IP-Ebene für den Tunnel.</span><span class="sxs-lookup"><span data-stu-id="0c2a4-120">Tunnel traffic at the IP layer.</span></span>|




