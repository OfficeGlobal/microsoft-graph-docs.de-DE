---
title: windowsInformationProtectionEnforcementLevel-Enumerationstyp
description: Mögliche Werte für Aktivierungs Ebenen für den WIP-Schutz
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1901059ef45141b0dc40d91dcbf4d9237cd6fc5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254814"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="afdb5-103">windowsInformationProtectionEnforcementLevel-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="afdb5-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="afdb5-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="afdb5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afdb5-105">Mögliche Werte für Aktivierungs Ebenen für den WIP-Schutz</span><span class="sxs-lookup"><span data-stu-id="afdb5-105">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="afdb5-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="afdb5-106">Members</span></span>
|<span data-ttu-id="afdb5-107">Element</span><span class="sxs-lookup"><span data-stu-id="afdb5-107">Member</span></span>|<span data-ttu-id="afdb5-108">Wert</span><span class="sxs-lookup"><span data-stu-id="afdb5-108">Value</span></span>|<span data-ttu-id="afdb5-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="afdb5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afdb5-110">noProtection</span><span class="sxs-lookup"><span data-stu-id="afdb5-110">noProtection</span></span>|<span data-ttu-id="afdb5-111">0</span><span class="sxs-lookup"><span data-stu-id="afdb5-111">0</span></span>|<span data-ttu-id="afdb5-112">Keine Schutz Erzwingung</span><span class="sxs-lookup"><span data-stu-id="afdb5-112">No protection enforcement</span></span>|
|<span data-ttu-id="afdb5-113">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="afdb5-113">encryptAndAuditOnly</span></span>|<span data-ttu-id="afdb5-114">1</span><span class="sxs-lookup"><span data-stu-id="afdb5-114">1</span></span>|<span data-ttu-id="afdb5-115">Nur verSchlüsseln und überWachen</span><span class="sxs-lookup"><span data-stu-id="afdb5-115">Encrypt and Audit only</span></span>|
|<span data-ttu-id="afdb5-116">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="afdb5-116">encryptAuditAndPrompt</span></span>|<span data-ttu-id="afdb5-117">2</span><span class="sxs-lookup"><span data-stu-id="afdb5-117">2</span></span>|<span data-ttu-id="afdb5-118">VerSchlüsseln, überWachen und anfordern</span><span class="sxs-lookup"><span data-stu-id="afdb5-118">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="afdb5-119">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="afdb5-119">encryptAuditAndBlock</span></span>|<span data-ttu-id="afdb5-120">3</span><span class="sxs-lookup"><span data-stu-id="afdb5-120">3</span></span>|<span data-ttu-id="afdb5-121">VerSchlüsseln, überWachen und blockieren</span><span class="sxs-lookup"><span data-stu-id="afdb5-121">Encrypt, Audit and Block</span></span>|



