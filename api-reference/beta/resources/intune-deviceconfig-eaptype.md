---
title: EapType Enum-Typ
description: Extensible Authentication-Protokoll (EAP) Konfigurationstypen.
author: tfitzmac
ms.openlocfilehash: e95924209b8137a1c5d35896c0195e9e962d7af9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319544"
---
# <a name="eaptype-enum-type"></a><span data-ttu-id="c1ce7-103">EapType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="c1ce7-103">eapType enum type</span></span>

> <span data-ttu-id="c1ce7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c1ce7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1ce7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c1ce7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1ce7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c1ce7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1ce7-107">Extensible Authentication-Protokoll (EAP) Konfigurationstypen.</span><span class="sxs-lookup"><span data-stu-id="c1ce7-107">Extensible Authentication Protocol (EAP) configuration types.</span></span>
## <a name="members"></a><span data-ttu-id="c1ce7-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="c1ce7-108">Members</span></span>
|<span data-ttu-id="c1ce7-109">Member</span><span class="sxs-lookup"><span data-stu-id="c1ce7-109">Member</span></span>|<span data-ttu-id="c1ce7-110">Wert</span><span class="sxs-lookup"><span data-stu-id="c1ce7-110">Value</span></span>|<span data-ttu-id="c1ce7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c1ce7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1ce7-112">eapTls</span><span class="sxs-lookup"><span data-stu-id="c1ce7-112">eapTls</span></span>|<span data-ttu-id="c1ce7-113">13</span><span class="sxs-lookup"><span data-stu-id="c1ce7-113">13</span></span>|<span data-ttu-id="c1ce7-114">EAP-Transport Layer Security (EAP-TLS).</span><span class="sxs-lookup"><span data-stu-id="c1ce7-114">EAP-Transport Layer Security (EAP-TLS).</span></span>|
|<span data-ttu-id="c1ce7-115">Sprung</span><span class="sxs-lookup"><span data-stu-id="c1ce7-115">leap</span></span>|<span data-ttu-id="c1ce7-116">17</span><span class="sxs-lookup"><span data-stu-id="c1ce7-116">17</span></span>|<span data-ttu-id="c1ce7-117">Einfache Extensible Authentication-Protokoll (SPRUNG).</span><span class="sxs-lookup"><span data-stu-id="c1ce7-117">Lightweight Extensible Authentication Protocol (LEAP).</span></span>|
|<span data-ttu-id="c1ce7-118">eapSim</span><span class="sxs-lookup"><span data-stu-id="c1ce7-118">eapSim</span></span>|<span data-ttu-id="c1ce7-119">18</span><span class="sxs-lookup"><span data-stu-id="c1ce7-119">18</span></span>|<span data-ttu-id="c1ce7-120">EAP für Zugriffszeichenfolge g/m2 (EAP-SIM).</span><span class="sxs-lookup"><span data-stu-id="c1ce7-120">EAP for GSM Subscriber Identity Module (EAP-SIM).</span></span>|
|<span data-ttu-id="c1ce7-121">eapTtls</span><span class="sxs-lookup"><span data-stu-id="c1ce7-121">eapTtls</span></span>|<span data-ttu-id="c1ce7-122">21</span><span class="sxs-lookup"><span data-stu-id="c1ce7-122">21</span></span>|<span data-ttu-id="c1ce7-123">EAP-getunnelt Transport Layer Security (EAP-TTLS).</span><span class="sxs-lookup"><span data-stu-id="c1ce7-123">EAP-Tunneled Transport Layer Security (EAP-TTLS).</span></span>|
|<span data-ttu-id="c1ce7-124">PEAP</span><span class="sxs-lookup"><span data-stu-id="c1ce7-124">peap</span></span>|<span data-ttu-id="c1ce7-125">25</span><span class="sxs-lookup"><span data-stu-id="c1ce7-125">25</span></span>|<span data-ttu-id="c1ce7-126">Extensible Authentication-Protokoll (PEAP) geschützt.</span><span class="sxs-lookup"><span data-stu-id="c1ce7-126">Protected Extensible Authentication Protocol (PEAP).</span></span>|
|<span data-ttu-id="c1ce7-127">eapFast</span><span class="sxs-lookup"><span data-stu-id="c1ce7-127">eapFast</span></span>|<span data-ttu-id="c1ce7-128">43</span><span class="sxs-lookup"><span data-stu-id="c1ce7-128">43</span></span>|<span data-ttu-id="c1ce7-129">EAP-Flexible Authentication via Secure Tunneling (EAP-FAST).</span><span class="sxs-lookup"><span data-stu-id="c1ce7-129">EAP-Flexible Authentication via Secure Tunneling (EAP-FAST).</span></span>|





