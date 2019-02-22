---
title: localSecurityOptionsMinimumSessionSecurity-Enumerationstyp
description: Mögliche Werte für LocalSecurityOptionsMinimumSessionSecurity
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe6007747aed1037a4dc3d5264bb432182a28c00
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145346"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="909e8-103">localSecurityOptionsMinimumSessionSecurity-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="909e8-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="909e8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="909e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="909e8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="909e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="909e8-106">Mögliche Werte für LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="909e8-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="909e8-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="909e8-107">Members</span></span>
|<span data-ttu-id="909e8-108">Element</span><span class="sxs-lookup"><span data-stu-id="909e8-108">Member</span></span>|<span data-ttu-id="909e8-109">Wert</span><span class="sxs-lookup"><span data-stu-id="909e8-109">Value</span></span>|<span data-ttu-id="909e8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="909e8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="909e8-111">Keine</span><span class="sxs-lookup"><span data-stu-id="909e8-111">none</span></span>|<span data-ttu-id="909e8-112">0</span><span class="sxs-lookup"><span data-stu-id="909e8-112">0</span></span>|<span data-ttu-id="909e8-113">Senden von LM-& NTLM-Antworten</span><span class="sxs-lookup"><span data-stu-id="909e8-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="909e8-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="909e8-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="909e8-115">1</span><span class="sxs-lookup"><span data-stu-id="909e8-115">1</span></span>|<span data-ttu-id="909e8-116">Senden von LM-& NTLM-Verwendung der NTLMv2-Sitzungssicherheit bei aushandeln</span><span class="sxs-lookup"><span data-stu-id="909e8-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="909e8-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="909e8-117">require128BitEncryption</span></span>|<span data-ttu-id="909e8-118">2</span><span class="sxs-lookup"><span data-stu-id="909e8-118">2</span></span>|<span data-ttu-id="909e8-119">Nur nur NTLM-Antworten für LM-& senden</span><span class="sxs-lookup"><span data-stu-id="909e8-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="909e8-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="909e8-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="909e8-121">3</span><span class="sxs-lookup"><span data-stu-id="909e8-121">3</span></span>|<span data-ttu-id="909e8-122">Nur LM-&-NTLMv2-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="909e8-122">Send LM & NTLMv2 responses only</span></span>|




