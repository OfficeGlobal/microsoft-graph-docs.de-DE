---
title: LanManagerAuthenticationLevel Enum-Typ
description: Mögliche Werte für LanManagerAuthenticationLevel
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 68af209a005dc1d7e8d25672f5e97e1d929ba25b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866913"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="d6c10-103">LanManagerAuthenticationLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="d6c10-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="d6c10-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d6c10-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6c10-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d6c10-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6c10-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d6c10-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6c10-107">Mögliche Werte für LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="d6c10-107">Possible values for LanManagerAuthenticationLevel</span></span>
## <a name="members"></a><span data-ttu-id="d6c10-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="d6c10-108">Members</span></span>
|<span data-ttu-id="d6c10-109">Element</span><span class="sxs-lookup"><span data-stu-id="d6c10-109">Member</span></span>|<span data-ttu-id="d6c10-110">Wert</span><span class="sxs-lookup"><span data-stu-id="d6c10-110">Value</span></span>|<span data-ttu-id="d6c10-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6c10-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6c10-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="d6c10-112">lmAndNltm</span></span>|<span data-ttu-id="d6c10-113">0</span><span class="sxs-lookup"><span data-stu-id="d6c10-113">0</span></span>|<span data-ttu-id="d6c10-114">LM & NTLM-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="d6c10-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="d6c10-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="d6c10-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="d6c10-116">1</span><span class="sxs-lookup"><span data-stu-id="d6c10-116">1</span></span>|<span data-ttu-id="d6c10-117">Senden Sie LM & NTLM-Verwendung NTLMv2 sitzungssicherheit, wenn ausgehandelt</span><span class="sxs-lookup"><span data-stu-id="d6c10-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="d6c10-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="d6c10-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="d6c10-119">2</span><span class="sxs-lookup"><span data-stu-id="d6c10-119">2</span></span>|<span data-ttu-id="d6c10-120">LM & NTLM-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="d6c10-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="d6c10-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="d6c10-121">lmAndNtlmV2</span></span>|<span data-ttu-id="d6c10-122">3</span><span class="sxs-lookup"><span data-stu-id="d6c10-122">3</span></span>|<span data-ttu-id="d6c10-123">LM & NTLMv2-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="d6c10-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="d6c10-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="d6c10-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="d6c10-125">4</span><span class="sxs-lookup"><span data-stu-id="d6c10-125">4</span></span>|<span data-ttu-id="d6c10-126">Senden Sie nur LM & NTLMv2-Antworten.</span><span class="sxs-lookup"><span data-stu-id="d6c10-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="d6c10-127">LM verweigern</span><span class="sxs-lookup"><span data-stu-id="d6c10-127">Refuse LM</span></span>|
|<span data-ttu-id="d6c10-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="d6c10-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="d6c10-129">5</span><span class="sxs-lookup"><span data-stu-id="d6c10-129">5</span></span>|<span data-ttu-id="d6c10-130">Senden Sie nur LM & NTLMv2-Antworten.</span><span class="sxs-lookup"><span data-stu-id="d6c10-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="d6c10-131">LM NTLM verweigern</span><span class="sxs-lookup"><span data-stu-id="d6c10-131">Refuse LM & NTLM</span></span>|





