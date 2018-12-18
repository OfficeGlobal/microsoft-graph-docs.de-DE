---
title: WiFiSecurityType Enum-Typ
description: Wi-Fi-Sicherheitstypen.
author: tfitzmac
ms.openlocfilehash: 291bc3660971a90ea113959368542e715a86b570
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329190"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="0e45c-103">WiFiSecurityType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="0e45c-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="0e45c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0e45c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e45c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0e45c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e45c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0e45c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e45c-107">Wi-Fi-Sicherheitstypen.</span><span class="sxs-lookup"><span data-stu-id="0e45c-107">Wi-Fi Security Types.</span></span>
## <a name="members"></a><span data-ttu-id="0e45c-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="0e45c-108">Members</span></span>
|<span data-ttu-id="0e45c-109">Member</span><span class="sxs-lookup"><span data-stu-id="0e45c-109">Member</span></span>|<span data-ttu-id="0e45c-110">Wert</span><span class="sxs-lookup"><span data-stu-id="0e45c-110">Value</span></span>|<span data-ttu-id="0e45c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e45c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e45c-112">Öffnen Sie</span><span class="sxs-lookup"><span data-stu-id="0e45c-112">open</span></span>|<span data-ttu-id="0e45c-113">0</span><span class="sxs-lookup"><span data-stu-id="0e45c-113">0</span></span>|<span data-ttu-id="0e45c-114">Öffnen Sie (keine Authentifizierung).</span><span class="sxs-lookup"><span data-stu-id="0e45c-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="0e45c-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="0e45c-115">wpaPersonal</span></span>|<span data-ttu-id="0e45c-116">1</span><span class="sxs-lookup"><span data-stu-id="0e45c-116">1</span></span>|<span data-ttu-id="0e45c-117">WPA-Persönlich.</span><span class="sxs-lookup"><span data-stu-id="0e45c-117">WPA-Personal.</span></span>|
|<span data-ttu-id="0e45c-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="0e45c-118">wpaEnterprise</span></span>|<span data-ttu-id="0e45c-119">2</span><span class="sxs-lookup"><span data-stu-id="0e45c-119">2</span></span>|<span data-ttu-id="0e45c-120">WPA-Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="0e45c-120">WPA-Enterprise.</span></span> <span data-ttu-id="0e45c-121">Muss einen IOSEnterpriseWifiConfiguration-Typ verwenden, um Enterprise-Optionen zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="0e45c-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="0e45c-122">WEP</span><span class="sxs-lookup"><span data-stu-id="0e45c-122">wep</span></span>|<span data-ttu-id="0e45c-123">3</span><span class="sxs-lookup"><span data-stu-id="0e45c-123">3</span></span>|<span data-ttu-id="0e45c-124">WEP-Verschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="0e45c-124">WEP Encryption.</span></span>|
|<span data-ttu-id="0e45c-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="0e45c-125">wpa2Personal</span></span>|<span data-ttu-id="0e45c-126">4</span><span class="sxs-lookup"><span data-stu-id="0e45c-126">4</span></span>|<span data-ttu-id="0e45c-127">WPA2-Persönlich.</span><span class="sxs-lookup"><span data-stu-id="0e45c-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="0e45c-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="0e45c-128">wpa2Enterprise</span></span>|<span data-ttu-id="0e45c-129">5</span><span class="sxs-lookup"><span data-stu-id="0e45c-129">5</span></span>|<span data-ttu-id="0e45c-130">WPA2-Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="0e45c-130">WPA2-Enterprise.</span></span> <span data-ttu-id="0e45c-131">Muss einen WindowsWifiEnterpriseEAPConfiguration-Typ verwenden, um Enterprise-Optionen zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="0e45c-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





