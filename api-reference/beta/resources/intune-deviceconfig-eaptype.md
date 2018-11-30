---
title: EapType Enum-Typ
description: Extensible Authentication-Protokoll (EAP) Konfigurationstypen.
ms.openlocfilehash: 871971878c741a8f7cd8a8f352e7b40e44562c38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058485"
---
# <a name="eaptype-enum-type"></a><span data-ttu-id="8d1e0-103">EapType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="8d1e0-103">eapType enum type</span></span>

> <span data-ttu-id="8d1e0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8d1e0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d1e0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8d1e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d1e0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8d1e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d1e0-107">Extensible Authentication-Protokoll (EAP) Konfigurationstypen.</span><span class="sxs-lookup"><span data-stu-id="8d1e0-107">Extensible Authentication Protocol (EAP) configuration types.</span></span>
## <a name="members"></a><span data-ttu-id="8d1e0-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="8d1e0-108">Members</span></span>
|<span data-ttu-id="8d1e0-109">Element</span><span class="sxs-lookup"><span data-stu-id="8d1e0-109">Member</span></span>|<span data-ttu-id="8d1e0-110">Wert</span><span class="sxs-lookup"><span data-stu-id="8d1e0-110">Value</span></span>|<span data-ttu-id="8d1e0-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d1e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d1e0-112">eapTls</span><span class="sxs-lookup"><span data-stu-id="8d1e0-112">eapTls</span></span>|<span data-ttu-id="8d1e0-113">13</span><span class="sxs-lookup"><span data-stu-id="8d1e0-113">13</span></span>|<span data-ttu-id="8d1e0-114">EAP-Transport Layer Security (EAP-TLS).</span><span class="sxs-lookup"><span data-stu-id="8d1e0-114">EAP-Transport Layer Security (EAP-TLS).</span></span>|
|<span data-ttu-id="8d1e0-115">Sprung</span><span class="sxs-lookup"><span data-stu-id="8d1e0-115">leap</span></span>|<span data-ttu-id="8d1e0-116">17</span><span class="sxs-lookup"><span data-stu-id="8d1e0-116">17</span></span>|<span data-ttu-id="8d1e0-117">Einfache Extensible Authentication-Protokoll (SPRUNG).</span><span class="sxs-lookup"><span data-stu-id="8d1e0-117">Lightweight Extensible Authentication Protocol (LEAP).</span></span>|
|<span data-ttu-id="8d1e0-118">eapSim</span><span class="sxs-lookup"><span data-stu-id="8d1e0-118">eapSim</span></span>|<span data-ttu-id="8d1e0-119">18</span><span class="sxs-lookup"><span data-stu-id="8d1e0-119">18</span></span>|<span data-ttu-id="8d1e0-120">EAP für Zugriffszeichenfolge g/m2 (EAP-SIM).</span><span class="sxs-lookup"><span data-stu-id="8d1e0-120">EAP for GSM Subscriber Identity Module (EAP-SIM).</span></span>|
|<span data-ttu-id="8d1e0-121">eapTtls</span><span class="sxs-lookup"><span data-stu-id="8d1e0-121">eapTtls</span></span>|<span data-ttu-id="8d1e0-122">21</span><span class="sxs-lookup"><span data-stu-id="8d1e0-122">21</span></span>|<span data-ttu-id="8d1e0-123">EAP-getunnelt Transport Layer Security (EAP-TTLS).</span><span class="sxs-lookup"><span data-stu-id="8d1e0-123">EAP-Tunneled Transport Layer Security (EAP-TTLS).</span></span>|
|<span data-ttu-id="8d1e0-124">PEAP</span><span class="sxs-lookup"><span data-stu-id="8d1e0-124">peap</span></span>|<span data-ttu-id="8d1e0-125">25</span><span class="sxs-lookup"><span data-stu-id="8d1e0-125">25</span></span>|<span data-ttu-id="8d1e0-126">Extensible Authentication-Protokoll (PEAP) geschützt.</span><span class="sxs-lookup"><span data-stu-id="8d1e0-126">Protected Extensible Authentication Protocol (PEAP).</span></span>|
|<span data-ttu-id="8d1e0-127">eapFast</span><span class="sxs-lookup"><span data-stu-id="8d1e0-127">eapFast</span></span>|<span data-ttu-id="8d1e0-128">43</span><span class="sxs-lookup"><span data-stu-id="8d1e0-128">43</span></span>|<span data-ttu-id="8d1e0-129">EAP-Flexible Authentication via Secure Tunneling (EAP-FAST).</span><span class="sxs-lookup"><span data-stu-id="8d1e0-129">EAP-Flexible Authentication via Secure Tunneling (EAP-FAST).</span></span>|





