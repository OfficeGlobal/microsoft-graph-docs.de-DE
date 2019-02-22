---
title: wiFiSecurityType-Enumerationstyp
description: WLAN-Sicherheitstypen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c16265ecf9b4fa56536838dde1f4f1f757d8b1f9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159045"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="4cfac-103">wiFiSecurityType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="4cfac-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="4cfac-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4cfac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cfac-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4cfac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cfac-106">WLAN-Sicherheitstypen.</span><span class="sxs-lookup"><span data-stu-id="4cfac-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="4cfac-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="4cfac-107">Members</span></span>
|<span data-ttu-id="4cfac-108">Element</span><span class="sxs-lookup"><span data-stu-id="4cfac-108">Member</span></span>|<span data-ttu-id="4cfac-109">Wert</span><span class="sxs-lookup"><span data-stu-id="4cfac-109">Value</span></span>|<span data-ttu-id="4cfac-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4cfac-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cfac-111">Öffnen</span><span class="sxs-lookup"><span data-stu-id="4cfac-111">open</span></span>|<span data-ttu-id="4cfac-112">0</span><span class="sxs-lookup"><span data-stu-id="4cfac-112">0</span></span>|<span data-ttu-id="4cfac-113">Open (keine Authentifizierung).</span><span class="sxs-lookup"><span data-stu-id="4cfac-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="4cfac-114">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="4cfac-114">wpaPersonal</span></span>|<span data-ttu-id="4cfac-115">1</span><span class="sxs-lookup"><span data-stu-id="4cfac-115">1</span></span>|<span data-ttu-id="4cfac-116">WPA-persönlich.</span><span class="sxs-lookup"><span data-stu-id="4cfac-116">WPA-Personal.</span></span>|
|<span data-ttu-id="4cfac-117">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="4cfac-117">wpaEnterprise</span></span>|<span data-ttu-id="4cfac-118">2</span><span class="sxs-lookup"><span data-stu-id="4cfac-118">2</span></span>|<span data-ttu-id="4cfac-119">WPA-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="4cfac-119">WPA-Enterprise.</span></span> <span data-ttu-id="4cfac-120">Verwenden Sie zum Konfigurieren von Enterprise-Optionen IOSEnterpriseWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4cfac-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="4cfac-121">WEP</span><span class="sxs-lookup"><span data-stu-id="4cfac-121">wep</span></span>|<span data-ttu-id="4cfac-122">3</span><span class="sxs-lookup"><span data-stu-id="4cfac-122">3</span></span>|<span data-ttu-id="4cfac-123">WEP-Verschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="4cfac-123">WEP Encryption.</span></span>|
|<span data-ttu-id="4cfac-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="4cfac-124">wpa2Personal</span></span>|<span data-ttu-id="4cfac-125">4</span><span class="sxs-lookup"><span data-stu-id="4cfac-125">4</span></span>|<span data-ttu-id="4cfac-126">WPA2-Persönlich.</span><span class="sxs-lookup"><span data-stu-id="4cfac-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="4cfac-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="4cfac-127">wpa2Enterprise</span></span>|<span data-ttu-id="4cfac-128">5</span><span class="sxs-lookup"><span data-stu-id="4cfac-128">5</span></span>|<span data-ttu-id="4cfac-129">WPA2-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="4cfac-129">WPA2-Enterprise.</span></span> <span data-ttu-id="4cfac-130">Verwenden Sie zum Konfigurieren von Enterprise-Optionen WindowsWifiEnterpriseEAPConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4cfac-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|




