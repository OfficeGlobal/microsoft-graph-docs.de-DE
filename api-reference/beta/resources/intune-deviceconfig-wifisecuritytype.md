---
title: WiFiSecurityType Enum-Typ
description: Wi-Fi-Sicherheitstypen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 73724041c223d50d0030bf27b780d6b694792a16
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422131"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="25d41-103">WiFiSecurityType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="25d41-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="25d41-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="25d41-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="25d41-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="25d41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25d41-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="25d41-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25d41-107">Wi-Fi-Sicherheitstypen.</span><span class="sxs-lookup"><span data-stu-id="25d41-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="25d41-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="25d41-108">Members</span></span>
|<span data-ttu-id="25d41-109">Member</span><span class="sxs-lookup"><span data-stu-id="25d41-109">Member</span></span>|<span data-ttu-id="25d41-110">Wert</span><span class="sxs-lookup"><span data-stu-id="25d41-110">Value</span></span>|<span data-ttu-id="25d41-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="25d41-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25d41-112">Öffnen Sie</span><span class="sxs-lookup"><span data-stu-id="25d41-112">open</span></span>|<span data-ttu-id="25d41-113">0</span><span class="sxs-lookup"><span data-stu-id="25d41-113">0</span></span>|<span data-ttu-id="25d41-114">Öffnen Sie (keine Authentifizierung).</span><span class="sxs-lookup"><span data-stu-id="25d41-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="25d41-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="25d41-115">wpaPersonal</span></span>|<span data-ttu-id="25d41-116">1</span><span class="sxs-lookup"><span data-stu-id="25d41-116">1</span></span>|<span data-ttu-id="25d41-117">WPA-Persönlich.</span><span class="sxs-lookup"><span data-stu-id="25d41-117">WPA-Personal.</span></span>|
|<span data-ttu-id="25d41-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="25d41-118">wpaEnterprise</span></span>|<span data-ttu-id="25d41-119">2</span><span class="sxs-lookup"><span data-stu-id="25d41-119">2</span></span>|<span data-ttu-id="25d41-120">WPA-Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="25d41-120">WPA-Enterprise.</span></span> <span data-ttu-id="25d41-121">Muss einen IOSEnterpriseWifiConfiguration-Typ verwenden, um Enterprise-Optionen zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="25d41-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="25d41-122">WEP</span><span class="sxs-lookup"><span data-stu-id="25d41-122">wep</span></span>|<span data-ttu-id="25d41-123">3</span><span class="sxs-lookup"><span data-stu-id="25d41-123">3</span></span>|<span data-ttu-id="25d41-124">WEP-Verschlüsselung.</span><span class="sxs-lookup"><span data-stu-id="25d41-124">WEP Encryption.</span></span>|
|<span data-ttu-id="25d41-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="25d41-125">wpa2Personal</span></span>|<span data-ttu-id="25d41-126">4</span><span class="sxs-lookup"><span data-stu-id="25d41-126">4</span></span>|<span data-ttu-id="25d41-127">WPA2-Persönlich.</span><span class="sxs-lookup"><span data-stu-id="25d41-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="25d41-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="25d41-128">wpa2Enterprise</span></span>|<span data-ttu-id="25d41-129">5</span><span class="sxs-lookup"><span data-stu-id="25d41-129">5</span></span>|<span data-ttu-id="25d41-130">WPA2-Unternehmen.</span><span class="sxs-lookup"><span data-stu-id="25d41-130">WPA2-Enterprise.</span></span> <span data-ttu-id="25d41-131">Muss einen WindowsWifiEnterpriseEAPConfiguration-Typ verwenden, um Enterprise-Optionen zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="25d41-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|




