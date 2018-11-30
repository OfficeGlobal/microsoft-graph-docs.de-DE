---
title: ComplianceState Enum-Typ
description: Compliance-Zustand.
ms.openlocfilehash: c49c0ecc2511f612e743fb5d86a53d150d3fbf45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064425"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="67ec3-103">ComplianceState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="67ec3-103">complianceState enum type</span></span>

> <span data-ttu-id="67ec3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="67ec3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67ec3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="67ec3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67ec3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="67ec3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67ec3-107">Compliance-Zustand.</span><span class="sxs-lookup"><span data-stu-id="67ec3-107">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="67ec3-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="67ec3-108">Members</span></span>
|<span data-ttu-id="67ec3-109">Element</span><span class="sxs-lookup"><span data-stu-id="67ec3-109">Member</span></span>|<span data-ttu-id="67ec3-110">Wert</span><span class="sxs-lookup"><span data-stu-id="67ec3-110">Value</span></span>|<span data-ttu-id="67ec3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67ec3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67ec3-112">unknown</span><span class="sxs-lookup"><span data-stu-id="67ec3-112">unknown</span></span>|<span data-ttu-id="67ec3-113">0</span><span class="sxs-lookup"><span data-stu-id="67ec3-113">0</span></span>|<span data-ttu-id="67ec3-114">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="67ec3-114">Unknown.</span></span>|
|<span data-ttu-id="67ec3-115">kompatible</span><span class="sxs-lookup"><span data-stu-id="67ec3-115">compliant</span></span>|<span data-ttu-id="67ec3-116">1</span><span class="sxs-lookup"><span data-stu-id="67ec3-116">1</span></span>|<span data-ttu-id="67ec3-117">Kompatibel.</span><span class="sxs-lookup"><span data-stu-id="67ec3-117">Compliant.</span></span>|
|<span data-ttu-id="67ec3-118">nicht konformer</span><span class="sxs-lookup"><span data-stu-id="67ec3-118">noncompliant</span></span>|<span data-ttu-id="67ec3-119">2</span><span class="sxs-lookup"><span data-stu-id="67ec3-119">2</span></span>|<span data-ttu-id="67ec3-120">Gerät ist nicht kompatibel und wird von Unternehmensressourcen blockiert.</span><span class="sxs-lookup"><span data-stu-id="67ec3-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="67ec3-121">Konflikt</span><span class="sxs-lookup"><span data-stu-id="67ec3-121">conflict</span></span>|<span data-ttu-id="67ec3-122">3</span><span class="sxs-lookup"><span data-stu-id="67ec3-122">3</span></span>|<span data-ttu-id="67ec3-123">Konflikt mit anderen Regeln.</span><span class="sxs-lookup"><span data-stu-id="67ec3-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="67ec3-124">error</span><span class="sxs-lookup"><span data-stu-id="67ec3-124">error</span></span>|<span data-ttu-id="67ec3-125">4</span><span class="sxs-lookup"><span data-stu-id="67ec3-125">4</span></span>|<span data-ttu-id="67ec3-126">Fehler</span><span class="sxs-lookup"><span data-stu-id="67ec3-126">Error.</span></span>|
|<span data-ttu-id="67ec3-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="67ec3-127">inGracePeriod</span></span>|<span data-ttu-id="67ec3-128">254</span><span class="sxs-lookup"><span data-stu-id="67ec3-128">254</span></span>|<span data-ttu-id="67ec3-129">Gerät nicht kompatibel ist, aber dennoch hat Zugriff auf Unternehmensressourcen</span><span class="sxs-lookup"><span data-stu-id="67ec3-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="67ec3-130">configManager</span><span class="sxs-lookup"><span data-stu-id="67ec3-130">configManager</span></span>|<span data-ttu-id="67ec3-131">255</span><span class="sxs-lookup"><span data-stu-id="67ec3-131">255</span></span>|<span data-ttu-id="67ec3-132">Vom Konfigurations-Manager verwaltet</span><span class="sxs-lookup"><span data-stu-id="67ec3-132">Managed by Config Manager</span></span>|





