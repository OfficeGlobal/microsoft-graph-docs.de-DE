---
title: LocalSecurityOptionsMinimumSessionSecurity Enum-Typ
description: Mögliche Werte für LocalSecurityOptionsMinimumSessionSecurity
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c39f2bb6d0bab2aff09fc05bb0492e81102e1b7c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396084"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="559cb-103">LocalSecurityOptionsMinimumSessionSecurity Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="559cb-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="559cb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="559cb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="559cb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="559cb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="559cb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="559cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="559cb-107">Mögliche Werte für LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="559cb-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="559cb-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="559cb-108">Members</span></span>
|<span data-ttu-id="559cb-109">Member</span><span class="sxs-lookup"><span data-stu-id="559cb-109">Member</span></span>|<span data-ttu-id="559cb-110">Wert</span><span class="sxs-lookup"><span data-stu-id="559cb-110">Value</span></span>|<span data-ttu-id="559cb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="559cb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="559cb-112">Keine</span><span class="sxs-lookup"><span data-stu-id="559cb-112">none</span></span>|<span data-ttu-id="559cb-113">0</span><span class="sxs-lookup"><span data-stu-id="559cb-113">0</span></span>|<span data-ttu-id="559cb-114">LM & NTLM-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="559cb-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="559cb-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="559cb-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="559cb-116">1</span><span class="sxs-lookup"><span data-stu-id="559cb-116">1</span></span>|<span data-ttu-id="559cb-117">Senden Sie LM & NTLM-Verwendung NTLMv2 sitzungssicherheit, wenn ausgehandelt</span><span class="sxs-lookup"><span data-stu-id="559cb-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="559cb-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="559cb-118">require128BitEncryption</span></span>|<span data-ttu-id="559cb-119">2</span><span class="sxs-lookup"><span data-stu-id="559cb-119">2</span></span>|<span data-ttu-id="559cb-120">LM & nur NTLM-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="559cb-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="559cb-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="559cb-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="559cb-122">3</span><span class="sxs-lookup"><span data-stu-id="559cb-122">3</span></span>|<span data-ttu-id="559cb-123">LM & nur NTLMv2-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="559cb-123">Send LM & NTLMv2 responses only</span></span>|




