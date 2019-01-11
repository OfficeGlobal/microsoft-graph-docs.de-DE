---
title: WindowsInformationProtectionEnforcementLevel Enum-Typ
description: Mögliche Werte für WIP Erzwingung Schutzebenen
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5097682172281ece366a8f0389c314e2fb630190
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868369"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="52f73-103">WindowsInformationProtectionEnforcementLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="52f73-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="52f73-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="52f73-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52f73-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="52f73-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52f73-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="52f73-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52f73-107">Mögliche Werte für WIP Erzwingung Schutzebenen</span><span class="sxs-lookup"><span data-stu-id="52f73-107">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="52f73-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="52f73-108">Members</span></span>
|<span data-ttu-id="52f73-109">Element</span><span class="sxs-lookup"><span data-stu-id="52f73-109">Member</span></span>|<span data-ttu-id="52f73-110">Wert</span><span class="sxs-lookup"><span data-stu-id="52f73-110">Value</span></span>|<span data-ttu-id="52f73-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52f73-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52f73-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="52f73-112">noProtection</span></span>|<span data-ttu-id="52f73-113">0</span><span class="sxs-lookup"><span data-stu-id="52f73-113">0</span></span>|<span data-ttu-id="52f73-114">Kein Schutz Erzwingung</span><span class="sxs-lookup"><span data-stu-id="52f73-114">No protection enforcement</span></span>|
|<span data-ttu-id="52f73-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="52f73-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="52f73-116">1</span><span class="sxs-lookup"><span data-stu-id="52f73-116">1</span></span>|<span data-ttu-id="52f73-117">Verschlüsseln und überwachen nur</span><span class="sxs-lookup"><span data-stu-id="52f73-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="52f73-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="52f73-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="52f73-119">2</span><span class="sxs-lookup"><span data-stu-id="52f73-119">2</span></span>|<span data-ttu-id="52f73-120">Verschlüsseln, überwachen und auffordern</span><span class="sxs-lookup"><span data-stu-id="52f73-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="52f73-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="52f73-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="52f73-122">3</span><span class="sxs-lookup"><span data-stu-id="52f73-122">3</span></span>|<span data-ttu-id="52f73-123">Verschlüsseln, überwachen und blockieren</span><span class="sxs-lookup"><span data-stu-id="52f73-123">Encrypt, Audit and Block</span></span>|





