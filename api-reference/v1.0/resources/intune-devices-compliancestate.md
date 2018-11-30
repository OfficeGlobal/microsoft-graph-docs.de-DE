---
title: ComplianceState Enum-Typ
description: Compliance-Zustand.
ms.openlocfilehash: 041a2267b952d37e0aeef29e1325e5cb7b561ed7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019465"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="e72db-103">ComplianceState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="e72db-103">complianceState enum type</span></span>

> <span data-ttu-id="e72db-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e72db-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e72db-105">Compliance-Zustand.</span><span class="sxs-lookup"><span data-stu-id="e72db-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="e72db-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="e72db-106">Members</span></span>
|<span data-ttu-id="e72db-107">Element</span><span class="sxs-lookup"><span data-stu-id="e72db-107">Member</span></span>|<span data-ttu-id="e72db-108">Wert</span><span class="sxs-lookup"><span data-stu-id="e72db-108">Value</span></span>|<span data-ttu-id="e72db-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e72db-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e72db-110">unknown</span><span class="sxs-lookup"><span data-stu-id="e72db-110">unknown</span></span>|<span data-ttu-id="e72db-111">0</span><span class="sxs-lookup"><span data-stu-id="e72db-111">0</span></span>|<span data-ttu-id="e72db-112">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="e72db-112">Unknown.</span></span>|
|<span data-ttu-id="e72db-113">kompatible</span><span class="sxs-lookup"><span data-stu-id="e72db-113">compliant</span></span>|<span data-ttu-id="e72db-114">1</span><span class="sxs-lookup"><span data-stu-id="e72db-114">1</span></span>|<span data-ttu-id="e72db-115">Kompatibel.</span><span class="sxs-lookup"><span data-stu-id="e72db-115">Compliant.</span></span>|
|<span data-ttu-id="e72db-116">nicht konformer</span><span class="sxs-lookup"><span data-stu-id="e72db-116">noncompliant</span></span>|<span data-ttu-id="e72db-117">2</span><span class="sxs-lookup"><span data-stu-id="e72db-117">2</span></span>|<span data-ttu-id="e72db-118">Gerät ist nicht kompatibel und wird von Unternehmensressourcen blockiert.</span><span class="sxs-lookup"><span data-stu-id="e72db-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="e72db-119">Konflikt</span><span class="sxs-lookup"><span data-stu-id="e72db-119">conflict</span></span>|<span data-ttu-id="e72db-120">3</span><span class="sxs-lookup"><span data-stu-id="e72db-120">3</span></span>|<span data-ttu-id="e72db-121">Konflikt mit anderen Regeln.</span><span class="sxs-lookup"><span data-stu-id="e72db-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="e72db-122">error</span><span class="sxs-lookup"><span data-stu-id="e72db-122">error</span></span>|<span data-ttu-id="e72db-123">4</span><span class="sxs-lookup"><span data-stu-id="e72db-123">4</span></span>|<span data-ttu-id="e72db-124">Fehler</span><span class="sxs-lookup"><span data-stu-id="e72db-124">Error.</span></span>|
|<span data-ttu-id="e72db-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="e72db-125">inGracePeriod</span></span>|<span data-ttu-id="e72db-126">254</span><span class="sxs-lookup"><span data-stu-id="e72db-126">254</span></span>|<span data-ttu-id="e72db-127">Gerät nicht kompatibel ist, aber dennoch hat Zugriff auf Unternehmensressourcen</span><span class="sxs-lookup"><span data-stu-id="e72db-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="e72db-128">configManager</span><span class="sxs-lookup"><span data-stu-id="e72db-128">configManager</span></span>|<span data-ttu-id="e72db-129">255</span><span class="sxs-lookup"><span data-stu-id="e72db-129">255</span></span>|<span data-ttu-id="e72db-130">Vom Konfigurations-Manager verwaltet</span><span class="sxs-lookup"><span data-stu-id="e72db-130">Managed by Config Manager</span></span>|



