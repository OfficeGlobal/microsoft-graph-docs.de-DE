---
title: complianceState-Enumerationstyp
description: Konformitätsstatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29357c5248aea78ffca8af464ecf4c3af17bdbc3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172926"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="5312a-103">complianceState-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="5312a-103">complianceState enum type</span></span>

> <span data-ttu-id="5312a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5312a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5312a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5312a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5312a-106">Konformitätsstatus.</span><span class="sxs-lookup"><span data-stu-id="5312a-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="5312a-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="5312a-107">Members</span></span>
|<span data-ttu-id="5312a-108">Element</span><span class="sxs-lookup"><span data-stu-id="5312a-108">Member</span></span>|<span data-ttu-id="5312a-109">Wert</span><span class="sxs-lookup"><span data-stu-id="5312a-109">Value</span></span>|<span data-ttu-id="5312a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5312a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5312a-111">unknown</span><span class="sxs-lookup"><span data-stu-id="5312a-111">unknown</span></span>|<span data-ttu-id="5312a-112">0</span><span class="sxs-lookup"><span data-stu-id="5312a-112">0</span></span>|<span data-ttu-id="5312a-113">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="5312a-113">Unknown.</span></span>|
|<span data-ttu-id="5312a-114">kompatibel</span><span class="sxs-lookup"><span data-stu-id="5312a-114">compliant</span></span>|<span data-ttu-id="5312a-115">1</span><span class="sxs-lookup"><span data-stu-id="5312a-115">1</span></span>|<span data-ttu-id="5312a-116">Kompatibel.</span><span class="sxs-lookup"><span data-stu-id="5312a-116">Compliant.</span></span>|
|<span data-ttu-id="5312a-117">konform</span><span class="sxs-lookup"><span data-stu-id="5312a-117">noncompliant</span></span>|<span data-ttu-id="5312a-118">2</span><span class="sxs-lookup"><span data-stu-id="5312a-118">2</span></span>|<span data-ttu-id="5312a-119">Das Gerät ist nicht kompatibel und wird von Unternehmensressourcen blockiert.</span><span class="sxs-lookup"><span data-stu-id="5312a-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="5312a-120">Konflikt</span><span class="sxs-lookup"><span data-stu-id="5312a-120">conflict</span></span>|<span data-ttu-id="5312a-121">3</span><span class="sxs-lookup"><span data-stu-id="5312a-121">3</span></span>|<span data-ttu-id="5312a-122">Konflikt mit anderen Regeln.</span><span class="sxs-lookup"><span data-stu-id="5312a-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="5312a-123">error</span><span class="sxs-lookup"><span data-stu-id="5312a-123">error</span></span>|<span data-ttu-id="5312a-124">4</span><span class="sxs-lookup"><span data-stu-id="5312a-124">4</span></span>|<span data-ttu-id="5312a-125">Fehler</span><span class="sxs-lookup"><span data-stu-id="5312a-125">Error.</span></span>|
|<span data-ttu-id="5312a-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="5312a-126">inGracePeriod</span></span>|<span data-ttu-id="5312a-127">254</span><span class="sxs-lookup"><span data-stu-id="5312a-127">254</span></span>|<span data-ttu-id="5312a-128">Das Gerät ist nicht kompatibel, hat jedoch weiterhin Zugriff auf Unternehmensressourcen.</span><span class="sxs-lookup"><span data-stu-id="5312a-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="5312a-129">configManager</span><span class="sxs-lookup"><span data-stu-id="5312a-129">configManager</span></span>|<span data-ttu-id="5312a-130">255</span><span class="sxs-lookup"><span data-stu-id="5312a-130">255</span></span>|<span data-ttu-id="5312a-131">Verwaltet von config Manager</span><span class="sxs-lookup"><span data-stu-id="5312a-131">Managed by Config Manager</span></span>|




