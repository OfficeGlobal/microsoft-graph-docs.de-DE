---
title: WiFiSecurityType Enum-Typ
description: Wi-Fi-Sicherheitstypen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6ddadaa31febaea08050ad49ffa540de53ff4819
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920219"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="7acb0-103">WiFiSecurityType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="7acb0-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="7acb0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7acb0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7acb0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7acb0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7acb0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7acb0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7acb0-107">Wi-Fi-Sicherheitstypen.</span><span class="sxs-lookup"><span data-stu-id="7acb0-107">Wi-Fi Security Types.</span></span>
## <a name="members"></a><span data-ttu-id="7acb0-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="7acb0-108">Members</span></span>
|<span data-ttu-id="7acb0-109">Element</span><span class="sxs-lookup"><span data-stu-id="7acb0-109">Member</span></span>|<span data-ttu-id="7acb0-110">Wert</span><span class="sxs-lookup"><span data-stu-id="7acb0-110">Value</span></span>|<span data-ttu-id="7acb0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7acb0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7acb0-112">Öffnen Sie</span><span class="sxs-lookup"><span data-stu-id="7acb0-112">open</span></span>|<span data-ttu-id="7acb0-113">0</span><span class="sxs-lookup"><span data-stu-id="7acb0-113">0</span></span>|<span data-ttu-id="7acb0-114">Öffnen Sie (keine Authentifizierung).</span><span class="sxs-lookup"><span data-stu-id="7acb0-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="7acb0-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="7acb0-115">wpaPersonal</span></span>|<span data-ttu-id="7acb0-116">1</span><span class="sxs-lookup"><span data-stu-id="7acb0-116">1</span></span>|<span data-ttu-id="7acb0-117">WPA-Persönlich.</span><span class="sxs-lookup"><span data-stu-id="7acb0-117">WPA-Personal.</span></span>|
|<span data-ttu-id="7acb0-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="7acb0-118">wpaEnterprise</span></span>|<span data-ttu-id="7acb0-119">2</span><span class="sxs-lookup"><span data-stu-id="7acb0-119">2</span></span>|<span data-ttu-id="7acb0-120">WPA-Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="7acb0-120">WPA-Enterprise.</span></span> <span data-ttu-id="7acb0-121">Muss einen IOSEnterpriseWifiConfiguration-Typ verwenden, um Enterprise-Optionen zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="7acb0-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="7acb0-122">WEP</span><span class="sxs-lookup"><span data-stu-id="7acb0-122">wep</span></span>|<span data-ttu-id="7acb0-123">3</span><span class="sxs-lookup"><span data-stu-id="7acb0-123">3</span></span>|<span data-ttu-id="7acb0-124">WEP-Verschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="7acb0-124">WEP Encryption.</span></span>|
|<span data-ttu-id="7acb0-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="7acb0-125">wpa2Personal</span></span>|<span data-ttu-id="7acb0-126">4</span><span class="sxs-lookup"><span data-stu-id="7acb0-126">4</span></span>|<span data-ttu-id="7acb0-127">WPA2-Persönlich.</span><span class="sxs-lookup"><span data-stu-id="7acb0-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="7acb0-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="7acb0-128">wpa2Enterprise</span></span>|<span data-ttu-id="7acb0-129">5</span><span class="sxs-lookup"><span data-stu-id="7acb0-129">5</span></span>|<span data-ttu-id="7acb0-130">WPA2-Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="7acb0-130">WPA2-Enterprise.</span></span> <span data-ttu-id="7acb0-131">Muss einen WindowsWifiEnterpriseEAPConfiguration-Typ verwenden, um Enterprise-Optionen zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="7acb0-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





