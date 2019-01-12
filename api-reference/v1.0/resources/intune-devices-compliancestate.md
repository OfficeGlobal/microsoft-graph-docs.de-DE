---
title: ComplianceState Enum-Typ
description: Compliance-Zustand.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5a4f4c359665eb1a0087f64802b5e7c829002fd6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940197"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="cba46-103">ComplianceState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="cba46-103">complianceState enum type</span></span>

> <span data-ttu-id="cba46-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cba46-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cba46-105">Compliance-Zustand.</span><span class="sxs-lookup"><span data-stu-id="cba46-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="cba46-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="cba46-106">Members</span></span>
|<span data-ttu-id="cba46-107">Element</span><span class="sxs-lookup"><span data-stu-id="cba46-107">Member</span></span>|<span data-ttu-id="cba46-108">Wert</span><span class="sxs-lookup"><span data-stu-id="cba46-108">Value</span></span>|<span data-ttu-id="cba46-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cba46-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cba46-110">unknown</span><span class="sxs-lookup"><span data-stu-id="cba46-110">unknown</span></span>|<span data-ttu-id="cba46-111">0</span><span class="sxs-lookup"><span data-stu-id="cba46-111">0</span></span>|<span data-ttu-id="cba46-112">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="cba46-112">Unknown.</span></span>|
|<span data-ttu-id="cba46-113">kompatible</span><span class="sxs-lookup"><span data-stu-id="cba46-113">compliant</span></span>|<span data-ttu-id="cba46-114">1</span><span class="sxs-lookup"><span data-stu-id="cba46-114">1</span></span>|<span data-ttu-id="cba46-115">Kompatibel.</span><span class="sxs-lookup"><span data-stu-id="cba46-115">Compliant.</span></span>|
|<span data-ttu-id="cba46-116">nicht konformer</span><span class="sxs-lookup"><span data-stu-id="cba46-116">noncompliant</span></span>|<span data-ttu-id="cba46-117">2</span><span class="sxs-lookup"><span data-stu-id="cba46-117">2</span></span>|<span data-ttu-id="cba46-118">Gerät ist nicht kompatibel und wird von Unternehmensressourcen blockiert.</span><span class="sxs-lookup"><span data-stu-id="cba46-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="cba46-119">Konflikt</span><span class="sxs-lookup"><span data-stu-id="cba46-119">conflict</span></span>|<span data-ttu-id="cba46-120">3</span><span class="sxs-lookup"><span data-stu-id="cba46-120">3</span></span>|<span data-ttu-id="cba46-121">Konflikt mit anderen Regeln.</span><span class="sxs-lookup"><span data-stu-id="cba46-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="cba46-122">error</span><span class="sxs-lookup"><span data-stu-id="cba46-122">error</span></span>|<span data-ttu-id="cba46-123">4</span><span class="sxs-lookup"><span data-stu-id="cba46-123">4</span></span>|<span data-ttu-id="cba46-124">Fehler</span><span class="sxs-lookup"><span data-stu-id="cba46-124">Error.</span></span>|
|<span data-ttu-id="cba46-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="cba46-125">inGracePeriod</span></span>|<span data-ttu-id="cba46-126">254</span><span class="sxs-lookup"><span data-stu-id="cba46-126">254</span></span>|<span data-ttu-id="cba46-127">Gerät nicht kompatibel ist, aber dennoch hat Zugriff auf Unternehmensressourcen</span><span class="sxs-lookup"><span data-stu-id="cba46-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="cba46-128">configManager</span><span class="sxs-lookup"><span data-stu-id="cba46-128">configManager</span></span>|<span data-ttu-id="cba46-129">255</span><span class="sxs-lookup"><span data-stu-id="cba46-129">255</span></span>|<span data-ttu-id="cba46-130">Vom Konfigurations-Manager verwaltet</span><span class="sxs-lookup"><span data-stu-id="cba46-130">Managed by Config Manager</span></span>|



