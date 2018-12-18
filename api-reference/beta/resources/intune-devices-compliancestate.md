---
title: ComplianceState Enum-Typ
description: Compliance-Zustand.
author: tfitzmac
ms.openlocfilehash: 3fa0548c2a67aa5def5f859014f52e97bdda815b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321231"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="4fa0e-103">ComplianceState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="4fa0e-103">complianceState enum type</span></span>

> <span data-ttu-id="4fa0e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4fa0e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4fa0e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4fa0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4fa0e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4fa0e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4fa0e-107">Compliance-Zustand.</span><span class="sxs-lookup"><span data-stu-id="4fa0e-107">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="4fa0e-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="4fa0e-108">Members</span></span>
|<span data-ttu-id="4fa0e-109">Member</span><span class="sxs-lookup"><span data-stu-id="4fa0e-109">Member</span></span>|<span data-ttu-id="4fa0e-110">Wert</span><span class="sxs-lookup"><span data-stu-id="4fa0e-110">Value</span></span>|<span data-ttu-id="4fa0e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4fa0e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fa0e-112">unknown</span><span class="sxs-lookup"><span data-stu-id="4fa0e-112">unknown</span></span>|<span data-ttu-id="4fa0e-113">0</span><span class="sxs-lookup"><span data-stu-id="4fa0e-113">0</span></span>|<span data-ttu-id="4fa0e-114">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="4fa0e-114">Unknown.</span></span>|
|<span data-ttu-id="4fa0e-115">kompatible</span><span class="sxs-lookup"><span data-stu-id="4fa0e-115">compliant</span></span>|<span data-ttu-id="4fa0e-116">1</span><span class="sxs-lookup"><span data-stu-id="4fa0e-116">1</span></span>|<span data-ttu-id="4fa0e-117">Kompatibel.</span><span class="sxs-lookup"><span data-stu-id="4fa0e-117">Compliant.</span></span>|
|<span data-ttu-id="4fa0e-118">nicht konformer</span><span class="sxs-lookup"><span data-stu-id="4fa0e-118">noncompliant</span></span>|<span data-ttu-id="4fa0e-119">2</span><span class="sxs-lookup"><span data-stu-id="4fa0e-119">2</span></span>|<span data-ttu-id="4fa0e-120">Gerät ist nicht kompatibel und wird von Unternehmensressourcen blockiert.</span><span class="sxs-lookup"><span data-stu-id="4fa0e-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="4fa0e-121">Konflikt</span><span class="sxs-lookup"><span data-stu-id="4fa0e-121">conflict</span></span>|<span data-ttu-id="4fa0e-122">3</span><span class="sxs-lookup"><span data-stu-id="4fa0e-122">3</span></span>|<span data-ttu-id="4fa0e-123">Konflikt mit anderen Regeln.</span><span class="sxs-lookup"><span data-stu-id="4fa0e-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="4fa0e-124">error</span><span class="sxs-lookup"><span data-stu-id="4fa0e-124">error</span></span>|<span data-ttu-id="4fa0e-125">4</span><span class="sxs-lookup"><span data-stu-id="4fa0e-125">4</span></span>|<span data-ttu-id="4fa0e-126">Fehler</span><span class="sxs-lookup"><span data-stu-id="4fa0e-126">Error.</span></span>|
|<span data-ttu-id="4fa0e-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="4fa0e-127">inGracePeriod</span></span>|<span data-ttu-id="4fa0e-128">254</span><span class="sxs-lookup"><span data-stu-id="4fa0e-128">254</span></span>|<span data-ttu-id="4fa0e-129">Gerät nicht kompatibel ist, aber dennoch hat Zugriff auf Unternehmensressourcen</span><span class="sxs-lookup"><span data-stu-id="4fa0e-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="4fa0e-130">configManager</span><span class="sxs-lookup"><span data-stu-id="4fa0e-130">configManager</span></span>|<span data-ttu-id="4fa0e-131">255</span><span class="sxs-lookup"><span data-stu-id="4fa0e-131">255</span></span>|<span data-ttu-id="4fa0e-132">Vom Konfigurations-Manager verwaltet</span><span class="sxs-lookup"><span data-stu-id="4fa0e-132">Managed by Config Manager</span></span>|





