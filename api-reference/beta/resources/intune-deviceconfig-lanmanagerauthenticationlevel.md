---
title: LanManagerAuthenticationLevel Enum-Typ
description: Mögliche Werte für LanManagerAuthenticationLevel
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6e8c7b3df6f515d3dad0d7619b6c0b755ad799d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397456"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="45a50-103">LanManagerAuthenticationLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="45a50-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="45a50-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="45a50-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="45a50-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="45a50-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45a50-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="45a50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45a50-107">Mögliche Werte für LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="45a50-107">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="45a50-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="45a50-108">Members</span></span>
|<span data-ttu-id="45a50-109">Member</span><span class="sxs-lookup"><span data-stu-id="45a50-109">Member</span></span>|<span data-ttu-id="45a50-110">Wert</span><span class="sxs-lookup"><span data-stu-id="45a50-110">Value</span></span>|<span data-ttu-id="45a50-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45a50-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45a50-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="45a50-112">lmAndNltm</span></span>|<span data-ttu-id="45a50-113">0</span><span class="sxs-lookup"><span data-stu-id="45a50-113">0</span></span>|<span data-ttu-id="45a50-114">LM & NTLM-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="45a50-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="45a50-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="45a50-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="45a50-116">1</span><span class="sxs-lookup"><span data-stu-id="45a50-116">1</span></span>|<span data-ttu-id="45a50-117">Senden Sie LM & NTLM-Verwendung NTLMv2 sitzungssicherheit, wenn ausgehandelt</span><span class="sxs-lookup"><span data-stu-id="45a50-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="45a50-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="45a50-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="45a50-119">2</span><span class="sxs-lookup"><span data-stu-id="45a50-119">2</span></span>|<span data-ttu-id="45a50-120">LM & nur NTLM-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="45a50-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="45a50-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="45a50-121">lmAndNtlmV2</span></span>|<span data-ttu-id="45a50-122">3</span><span class="sxs-lookup"><span data-stu-id="45a50-122">3</span></span>|<span data-ttu-id="45a50-123">LM & nur NTLMv2-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="45a50-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="45a50-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="45a50-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="45a50-125">4</span><span class="sxs-lookup"><span data-stu-id="45a50-125">4</span></span>|<span data-ttu-id="45a50-126">Senden Sie LM & nur die NTLMv2-Antworten.</span><span class="sxs-lookup"><span data-stu-id="45a50-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="45a50-127">LM verweigern</span><span class="sxs-lookup"><span data-stu-id="45a50-127">Refuse LM</span></span>|
|<span data-ttu-id="45a50-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="45a50-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="45a50-129">5</span><span class="sxs-lookup"><span data-stu-id="45a50-129">5</span></span>|<span data-ttu-id="45a50-130">Senden Sie LM & nur die NTLMv2-Antworten.</span><span class="sxs-lookup"><span data-stu-id="45a50-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="45a50-131">LM & NTLM verweigern</span><span class="sxs-lookup"><span data-stu-id="45a50-131">Refuse LM & NTLM</span></span>|




