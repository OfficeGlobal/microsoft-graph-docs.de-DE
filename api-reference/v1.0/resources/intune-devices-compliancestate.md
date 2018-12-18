---
title: ComplianceState Enum-Typ
description: Compliance-Zustand.
author: tfitzmac
ms.openlocfilehash: 3045685518f1c7718f9a5f46cd10e0add6fe05b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330275"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="c67e4-103">ComplianceState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="c67e4-103">complianceState enum type</span></span>

> <span data-ttu-id="c67e4-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c67e4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c67e4-105">Compliance-Zustand.</span><span class="sxs-lookup"><span data-stu-id="c67e4-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="c67e4-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="c67e4-106">Members</span></span>
|<span data-ttu-id="c67e4-107">Member</span><span class="sxs-lookup"><span data-stu-id="c67e4-107">Member</span></span>|<span data-ttu-id="c67e4-108">Wert</span><span class="sxs-lookup"><span data-stu-id="c67e4-108">Value</span></span>|<span data-ttu-id="c67e4-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c67e4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c67e4-110">unknown</span><span class="sxs-lookup"><span data-stu-id="c67e4-110">unknown</span></span>|<span data-ttu-id="c67e4-111">0</span><span class="sxs-lookup"><span data-stu-id="c67e4-111">0</span></span>|<span data-ttu-id="c67e4-112">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="c67e4-112">Unknown.</span></span>|
|<span data-ttu-id="c67e4-113">kompatible</span><span class="sxs-lookup"><span data-stu-id="c67e4-113">compliant</span></span>|<span data-ttu-id="c67e4-114">1</span><span class="sxs-lookup"><span data-stu-id="c67e4-114">1</span></span>|<span data-ttu-id="c67e4-115">Kompatibel.</span><span class="sxs-lookup"><span data-stu-id="c67e4-115">Compliant.</span></span>|
|<span data-ttu-id="c67e4-116">nicht konformer</span><span class="sxs-lookup"><span data-stu-id="c67e4-116">noncompliant</span></span>|<span data-ttu-id="c67e4-117">2</span><span class="sxs-lookup"><span data-stu-id="c67e4-117">2</span></span>|<span data-ttu-id="c67e4-118">Gerät ist nicht kompatibel und wird von Unternehmensressourcen blockiert.</span><span class="sxs-lookup"><span data-stu-id="c67e4-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="c67e4-119">Konflikt</span><span class="sxs-lookup"><span data-stu-id="c67e4-119">conflict</span></span>|<span data-ttu-id="c67e4-120">3</span><span class="sxs-lookup"><span data-stu-id="c67e4-120">3</span></span>|<span data-ttu-id="c67e4-121">Konflikt mit anderen Regeln.</span><span class="sxs-lookup"><span data-stu-id="c67e4-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="c67e4-122">error</span><span class="sxs-lookup"><span data-stu-id="c67e4-122">error</span></span>|<span data-ttu-id="c67e4-123">4</span><span class="sxs-lookup"><span data-stu-id="c67e4-123">4</span></span>|<span data-ttu-id="c67e4-124">Fehler</span><span class="sxs-lookup"><span data-stu-id="c67e4-124">Error.</span></span>|
|<span data-ttu-id="c67e4-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="c67e4-125">inGracePeriod</span></span>|<span data-ttu-id="c67e4-126">254</span><span class="sxs-lookup"><span data-stu-id="c67e4-126">254</span></span>|<span data-ttu-id="c67e4-127">Gerät nicht kompatibel ist, aber dennoch hat Zugriff auf Unternehmensressourcen</span><span class="sxs-lookup"><span data-stu-id="c67e4-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="c67e4-128">configManager</span><span class="sxs-lookup"><span data-stu-id="c67e4-128">configManager</span></span>|<span data-ttu-id="c67e4-129">255</span><span class="sxs-lookup"><span data-stu-id="c67e4-129">255</span></span>|<span data-ttu-id="c67e4-130">Vom Konfigurations-Manager verwaltet</span><span class="sxs-lookup"><span data-stu-id="c67e4-130">Managed by Config Manager</span></span>|



