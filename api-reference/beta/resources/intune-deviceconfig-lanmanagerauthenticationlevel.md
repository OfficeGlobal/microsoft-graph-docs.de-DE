---
title: LanManagerAuthenticationLevel Enum-Typ
description: Mögliche Werte für LanManagerAuthenticationLevel
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fd88deb7684301023a75905d12a59ce25bad750f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911994"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="65692-103">LanManagerAuthenticationLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="65692-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="65692-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="65692-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65692-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="65692-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65692-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="65692-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65692-107">Mögliche Werte für LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="65692-107">Possible values for LanManagerAuthenticationLevel</span></span>
## <a name="members"></a><span data-ttu-id="65692-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="65692-108">Members</span></span>
|<span data-ttu-id="65692-109">Element</span><span class="sxs-lookup"><span data-stu-id="65692-109">Member</span></span>|<span data-ttu-id="65692-110">Wert</span><span class="sxs-lookup"><span data-stu-id="65692-110">Value</span></span>|<span data-ttu-id="65692-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65692-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65692-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="65692-112">lmAndNltm</span></span>|<span data-ttu-id="65692-113">0</span><span class="sxs-lookup"><span data-stu-id="65692-113">0</span></span>|<span data-ttu-id="65692-114">LM & NTLM-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="65692-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="65692-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="65692-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="65692-116">1</span><span class="sxs-lookup"><span data-stu-id="65692-116">1</span></span>|<span data-ttu-id="65692-117">Senden Sie LM & NTLM-Verwendung NTLMv2 sitzungssicherheit, wenn ausgehandelt</span><span class="sxs-lookup"><span data-stu-id="65692-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="65692-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="65692-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="65692-119">2</span><span class="sxs-lookup"><span data-stu-id="65692-119">2</span></span>|<span data-ttu-id="65692-120">LM & NTLM-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="65692-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="65692-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="65692-121">lmAndNtlmV2</span></span>|<span data-ttu-id="65692-122">3</span><span class="sxs-lookup"><span data-stu-id="65692-122">3</span></span>|<span data-ttu-id="65692-123">LM & NTLMv2-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="65692-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="65692-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="65692-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="65692-125">4</span><span class="sxs-lookup"><span data-stu-id="65692-125">4</span></span>|<span data-ttu-id="65692-126">Senden Sie nur LM & NTLMv2-Antworten.</span><span class="sxs-lookup"><span data-stu-id="65692-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="65692-127">LM verweigern</span><span class="sxs-lookup"><span data-stu-id="65692-127">Refuse LM</span></span>|
|<span data-ttu-id="65692-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="65692-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="65692-129">5</span><span class="sxs-lookup"><span data-stu-id="65692-129">5</span></span>|<span data-ttu-id="65692-130">Senden Sie nur LM & NTLMv2-Antworten.</span><span class="sxs-lookup"><span data-stu-id="65692-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="65692-131">LM NTLM verweigern</span><span class="sxs-lookup"><span data-stu-id="65692-131">Refuse LM & NTLM</span></span>|





