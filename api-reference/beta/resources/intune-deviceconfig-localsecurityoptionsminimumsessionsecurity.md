---
title: LocalSecurityOptionsMinimumSessionSecurity Enum-Typ
description: Mögliche Werte für LocalSecurityOptionsMinimumSessionSecurity
author: tfitzmac
ms.openlocfilehash: 5feabd9c84ec42f55bb45b952be5af834fd84498
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350631"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="16225-103">LocalSecurityOptionsMinimumSessionSecurity Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="16225-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="16225-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="16225-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16225-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16225-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16225-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="16225-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16225-107">Mögliche Werte für LocalSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="16225-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>
## <a name="members"></a><span data-ttu-id="16225-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="16225-108">Members</span></span>
|<span data-ttu-id="16225-109">Member</span><span class="sxs-lookup"><span data-stu-id="16225-109">Member</span></span>|<span data-ttu-id="16225-110">Wert</span><span class="sxs-lookup"><span data-stu-id="16225-110">Value</span></span>|<span data-ttu-id="16225-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16225-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16225-112">Keine</span><span class="sxs-lookup"><span data-stu-id="16225-112">none</span></span>|<span data-ttu-id="16225-113">0</span><span class="sxs-lookup"><span data-stu-id="16225-113">0</span></span>|<span data-ttu-id="16225-114">LM & NTLM-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="16225-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="16225-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="16225-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="16225-116">1</span><span class="sxs-lookup"><span data-stu-id="16225-116">1</span></span>|<span data-ttu-id="16225-117">Senden Sie LM & NTLM-Verwendung NTLMv2 sitzungssicherheit, wenn ausgehandelt</span><span class="sxs-lookup"><span data-stu-id="16225-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="16225-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="16225-118">require128BitEncryption</span></span>|<span data-ttu-id="16225-119">2</span><span class="sxs-lookup"><span data-stu-id="16225-119">2</span></span>|<span data-ttu-id="16225-120">LM & NTLM-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="16225-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="16225-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="16225-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="16225-122">3</span><span class="sxs-lookup"><span data-stu-id="16225-122">3</span></span>|<span data-ttu-id="16225-123">LM & NTLMv2-Antworten senden</span><span class="sxs-lookup"><span data-stu-id="16225-123">Send LM & NTLMv2 responses only</span></span>|





