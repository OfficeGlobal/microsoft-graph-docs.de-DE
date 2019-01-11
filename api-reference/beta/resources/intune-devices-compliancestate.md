---
title: ComplianceState Enum-Typ
description: Compliance-Zustand.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b3d496d6890d0da4d817ad9ba1f03e4b0825204d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861677"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="5a0af-103">ComplianceState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="5a0af-103">complianceState enum type</span></span>

> <span data-ttu-id="5a0af-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5a0af-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a0af-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5a0af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a0af-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5a0af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a0af-107">Compliance-Zustand.</span><span class="sxs-lookup"><span data-stu-id="5a0af-107">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="5a0af-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="5a0af-108">Members</span></span>
|<span data-ttu-id="5a0af-109">Element</span><span class="sxs-lookup"><span data-stu-id="5a0af-109">Member</span></span>|<span data-ttu-id="5a0af-110">Wert</span><span class="sxs-lookup"><span data-stu-id="5a0af-110">Value</span></span>|<span data-ttu-id="5a0af-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5a0af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a0af-112">unknown</span><span class="sxs-lookup"><span data-stu-id="5a0af-112">unknown</span></span>|<span data-ttu-id="5a0af-113">0</span><span class="sxs-lookup"><span data-stu-id="5a0af-113">0</span></span>|<span data-ttu-id="5a0af-114">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="5a0af-114">Unknown.</span></span>|
|<span data-ttu-id="5a0af-115">kompatible</span><span class="sxs-lookup"><span data-stu-id="5a0af-115">compliant</span></span>|<span data-ttu-id="5a0af-116">1</span><span class="sxs-lookup"><span data-stu-id="5a0af-116">1</span></span>|<span data-ttu-id="5a0af-117">Kompatibel.</span><span class="sxs-lookup"><span data-stu-id="5a0af-117">Compliant.</span></span>|
|<span data-ttu-id="5a0af-118">nicht konformer</span><span class="sxs-lookup"><span data-stu-id="5a0af-118">noncompliant</span></span>|<span data-ttu-id="5a0af-119">2</span><span class="sxs-lookup"><span data-stu-id="5a0af-119">2</span></span>|<span data-ttu-id="5a0af-120">Gerät ist nicht kompatibel und wird von Unternehmensressourcen blockiert.</span><span class="sxs-lookup"><span data-stu-id="5a0af-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="5a0af-121">Konflikt</span><span class="sxs-lookup"><span data-stu-id="5a0af-121">conflict</span></span>|<span data-ttu-id="5a0af-122">3</span><span class="sxs-lookup"><span data-stu-id="5a0af-122">3</span></span>|<span data-ttu-id="5a0af-123">Konflikt mit anderen Regeln.</span><span class="sxs-lookup"><span data-stu-id="5a0af-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="5a0af-124">error</span><span class="sxs-lookup"><span data-stu-id="5a0af-124">error</span></span>|<span data-ttu-id="5a0af-125">4</span><span class="sxs-lookup"><span data-stu-id="5a0af-125">4</span></span>|<span data-ttu-id="5a0af-126">Fehler</span><span class="sxs-lookup"><span data-stu-id="5a0af-126">Error.</span></span>|
|<span data-ttu-id="5a0af-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="5a0af-127">inGracePeriod</span></span>|<span data-ttu-id="5a0af-128">254</span><span class="sxs-lookup"><span data-stu-id="5a0af-128">254</span></span>|<span data-ttu-id="5a0af-129">Gerät nicht kompatibel ist, aber dennoch hat Zugriff auf Unternehmensressourcen</span><span class="sxs-lookup"><span data-stu-id="5a0af-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="5a0af-130">configManager</span><span class="sxs-lookup"><span data-stu-id="5a0af-130">configManager</span></span>|<span data-ttu-id="5a0af-131">255</span><span class="sxs-lookup"><span data-stu-id="5a0af-131">255</span></span>|<span data-ttu-id="5a0af-132">Vom Konfigurations-Manager verwaltet</span><span class="sxs-lookup"><span data-stu-id="5a0af-132">Managed by Config Manager</span></span>|





