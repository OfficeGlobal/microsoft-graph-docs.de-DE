---
title: lanManagerAuthenticationLevel-Enumerationstyp
description: Mögliche Werte für LanManagerAuthenticationLevel
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63f04f1ef2fc12fa0352aeec803c46fb4ebab3d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166570"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="1f3a0-103">lanManagerAuthenticationLevel-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="1f3a0-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="1f3a0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1f3a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f3a0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1f3a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f3a0-106">Mögliche Werte für LanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="1f3a0-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="1f3a0-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="1f3a0-107">Members</span></span>
|<span data-ttu-id="1f3a0-108">Element</span><span class="sxs-lookup"><span data-stu-id="1f3a0-108">Member</span></span>|<span data-ttu-id="1f3a0-109">Wert</span><span class="sxs-lookup"><span data-stu-id="1f3a0-109">Value</span></span>|<span data-ttu-id="1f3a0-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f3a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f3a0-111">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="1f3a0-111">lmAndNltm</span></span>|<span data-ttu-id="1f3a0-112">0</span><span class="sxs-lookup"><span data-stu-id="1f3a0-112">0</span></span>|<span data-ttu-id="1f3a0-113">Senden von LM-& NTLM-Antworten</span><span class="sxs-lookup"><span data-stu-id="1f3a0-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="1f3a0-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="1f3a0-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="1f3a0-115">1</span><span class="sxs-lookup"><span data-stu-id="1f3a0-115">1</span></span>|<span data-ttu-id="1f3a0-116">Senden von LM-& NTLM-Verwendung der NTLMv2-Sitzungssicherheit bei aushandeln</span><span class="sxs-lookup"><span data-stu-id="1f3a0-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="1f3a0-117">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="1f3a0-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="1f3a0-118">2</span><span class="sxs-lookup"><span data-stu-id="1f3a0-118">2</span></span>|<span data-ttu-id="1f3a0-119">Nur nur NTLM-Antworten für LM-& senden</span><span class="sxs-lookup"><span data-stu-id="1f3a0-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="1f3a0-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="1f3a0-120">lmAndNtlmV2</span></span>|<span data-ttu-id="1f3a0-121">3</span><span class="sxs-lookup"><span data-stu-id="1f3a0-121">3</span></span>|<span data-ttu-id="1f3a0-122">Nur LM-&-NTLMv2-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="1f3a0-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="1f3a0-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="1f3a0-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="1f3a0-124">4</span><span class="sxs-lookup"><span data-stu-id="1f3a0-124">4</span></span>|<span data-ttu-id="1f3a0-125">Senden Sie nur LINEARe &-NTLMv2-Antworten.</span><span class="sxs-lookup"><span data-stu-id="1f3a0-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="1f3a0-126">LM ablehnen</span><span class="sxs-lookup"><span data-stu-id="1f3a0-126">Refuse LM</span></span>|
|<span data-ttu-id="1f3a0-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="1f3a0-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="1f3a0-128">5</span><span class="sxs-lookup"><span data-stu-id="1f3a0-128">5</span></span>|<span data-ttu-id="1f3a0-129">Senden Sie nur LINEARe &-NTLMv2-Antworten.</span><span class="sxs-lookup"><span data-stu-id="1f3a0-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="1f3a0-130">Ablehnen von LM & NTLM</span><span class="sxs-lookup"><span data-stu-id="1f3a0-130">Refuse LM & NTLM</span></span>|




