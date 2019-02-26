---
title: windowsInformationProtectionEnforcementLevel-Enumerationstyp
description: Mögliche Werte für Aktivierungs Ebenen für den WIP-Schutz
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 184f5b6d296a37f9356c2cfeefe7c3ecdbdb6973
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150148"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="0c185-103">windowsInformationProtectionEnforcementLevel-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="0c185-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="0c185-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0c185-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c185-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0c185-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c185-106">Mögliche Werte für Aktivierungs Ebenen für den WIP-Schutz</span><span class="sxs-lookup"><span data-stu-id="0c185-106">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="0c185-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="0c185-107">Members</span></span>
|<span data-ttu-id="0c185-108">Element</span><span class="sxs-lookup"><span data-stu-id="0c185-108">Member</span></span>|<span data-ttu-id="0c185-109">Wert</span><span class="sxs-lookup"><span data-stu-id="0c185-109">Value</span></span>|<span data-ttu-id="0c185-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c185-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c185-111">noProtection</span><span class="sxs-lookup"><span data-stu-id="0c185-111">noProtection</span></span>|<span data-ttu-id="0c185-112">0</span><span class="sxs-lookup"><span data-stu-id="0c185-112">0</span></span>|<span data-ttu-id="0c185-113">Keine Schutz Erzwingung</span><span class="sxs-lookup"><span data-stu-id="0c185-113">No protection enforcement</span></span>|
|<span data-ttu-id="0c185-114">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="0c185-114">encryptAndAuditOnly</span></span>|<span data-ttu-id="0c185-115">1</span><span class="sxs-lookup"><span data-stu-id="0c185-115">1</span></span>|<span data-ttu-id="0c185-116">Nur verSchlüsseln und überWachen</span><span class="sxs-lookup"><span data-stu-id="0c185-116">Encrypt and Audit only</span></span>|
|<span data-ttu-id="0c185-117">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="0c185-117">encryptAuditAndPrompt</span></span>|<span data-ttu-id="0c185-118">2</span><span class="sxs-lookup"><span data-stu-id="0c185-118">2</span></span>|<span data-ttu-id="0c185-119">VerSchlüsseln, überWachen und anfordern</span><span class="sxs-lookup"><span data-stu-id="0c185-119">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="0c185-120">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="0c185-120">encryptAuditAndBlock</span></span>|<span data-ttu-id="0c185-121">3</span><span class="sxs-lookup"><span data-stu-id="0c185-121">3</span></span>|<span data-ttu-id="0c185-122">VerSchlüsseln, überWachen und blockieren</span><span class="sxs-lookup"><span data-stu-id="0c185-122">Encrypt, Audit and Block</span></span>|




