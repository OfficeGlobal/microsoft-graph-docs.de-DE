---
title: vpnProviderType-Enumerationstyp
description: Anbietertyp für pro-App-VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a62436f56a210bbb71606ebb8f2586e5b48f8d1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163189"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="13b05-103">vpnProviderType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="13b05-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="13b05-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13b05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13b05-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="13b05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13b05-106">Anbietertyp für pro-App-VPN.</span><span class="sxs-lookup"><span data-stu-id="13b05-106">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="13b05-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="13b05-107">Members</span></span>
|<span data-ttu-id="13b05-108">Element</span><span class="sxs-lookup"><span data-stu-id="13b05-108">Member</span></span>|<span data-ttu-id="13b05-109">Wert</span><span class="sxs-lookup"><span data-stu-id="13b05-109">Value</span></span>|<span data-ttu-id="13b05-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13b05-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13b05-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="13b05-111">notConfigured</span></span>|<span data-ttu-id="13b05-112">0</span><span class="sxs-lookup"><span data-stu-id="13b05-112">0</span></span>|<span data-ttu-id="13b05-113">Tunnel Datenverkehr wird nicht explizit konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="13b05-113">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="13b05-114">appProxy</span><span class="sxs-lookup"><span data-stu-id="13b05-114">appProxy</span></span>|<span data-ttu-id="13b05-115">1</span><span class="sxs-lookup"><span data-stu-id="13b05-115">1</span></span>|<span data-ttu-id="13b05-116">Tunnel Datenverkehr auf der Anwendungsebene</span><span class="sxs-lookup"><span data-stu-id="13b05-116">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="13b05-117">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="13b05-117">packetTunnel</span></span>|<span data-ttu-id="13b05-118">2</span><span class="sxs-lookup"><span data-stu-id="13b05-118">2</span></span>|<span data-ttu-id="13b05-119">Tunnel Datenverkehr auf der IP-Ebene.</span><span class="sxs-lookup"><span data-stu-id="13b05-119">Tunnel traffic at the IP layer.</span></span>|




