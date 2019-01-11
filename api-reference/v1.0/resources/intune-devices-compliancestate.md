---
title: ComplianceState Enum-Typ
description: Compliance-Zustand.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53b17f258f577e0842dbfc81c6341303f6b43799
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820342"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="8c973-103">ComplianceState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="8c973-103">complianceState enum type</span></span>

> <span data-ttu-id="8c973-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8c973-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c973-105">Compliance-Zustand.</span><span class="sxs-lookup"><span data-stu-id="8c973-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="8c973-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="8c973-106">Members</span></span>
|<span data-ttu-id="8c973-107">Element</span><span class="sxs-lookup"><span data-stu-id="8c973-107">Member</span></span>|<span data-ttu-id="8c973-108">Wert</span><span class="sxs-lookup"><span data-stu-id="8c973-108">Value</span></span>|<span data-ttu-id="8c973-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c973-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c973-110">unknown</span><span class="sxs-lookup"><span data-stu-id="8c973-110">unknown</span></span>|<span data-ttu-id="8c973-111">0</span><span class="sxs-lookup"><span data-stu-id="8c973-111">0</span></span>|<span data-ttu-id="8c973-112">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="8c973-112">Unknown.</span></span>|
|<span data-ttu-id="8c973-113">kompatible</span><span class="sxs-lookup"><span data-stu-id="8c973-113">compliant</span></span>|<span data-ttu-id="8c973-114">1</span><span class="sxs-lookup"><span data-stu-id="8c973-114">1</span></span>|<span data-ttu-id="8c973-115">Kompatibel.</span><span class="sxs-lookup"><span data-stu-id="8c973-115">Compliant.</span></span>|
|<span data-ttu-id="8c973-116">nicht konformer</span><span class="sxs-lookup"><span data-stu-id="8c973-116">noncompliant</span></span>|<span data-ttu-id="8c973-117">2</span><span class="sxs-lookup"><span data-stu-id="8c973-117">2</span></span>|<span data-ttu-id="8c973-118">Gerät ist nicht kompatibel und wird von Unternehmensressourcen blockiert.</span><span class="sxs-lookup"><span data-stu-id="8c973-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="8c973-119">Konflikt</span><span class="sxs-lookup"><span data-stu-id="8c973-119">conflict</span></span>|<span data-ttu-id="8c973-120">3</span><span class="sxs-lookup"><span data-stu-id="8c973-120">3</span></span>|<span data-ttu-id="8c973-121">Konflikt mit anderen Regeln.</span><span class="sxs-lookup"><span data-stu-id="8c973-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="8c973-122">error</span><span class="sxs-lookup"><span data-stu-id="8c973-122">error</span></span>|<span data-ttu-id="8c973-123">4</span><span class="sxs-lookup"><span data-stu-id="8c973-123">4</span></span>|<span data-ttu-id="8c973-124">Fehler</span><span class="sxs-lookup"><span data-stu-id="8c973-124">Error.</span></span>|
|<span data-ttu-id="8c973-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="8c973-125">inGracePeriod</span></span>|<span data-ttu-id="8c973-126">254</span><span class="sxs-lookup"><span data-stu-id="8c973-126">254</span></span>|<span data-ttu-id="8c973-127">Gerät nicht kompatibel ist, aber dennoch hat Zugriff auf Unternehmensressourcen</span><span class="sxs-lookup"><span data-stu-id="8c973-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="8c973-128">configManager</span><span class="sxs-lookup"><span data-stu-id="8c973-128">configManager</span></span>|<span data-ttu-id="8c973-129">255</span><span class="sxs-lookup"><span data-stu-id="8c973-129">255</span></span>|<span data-ttu-id="8c973-130">Vom Konfigurations-Manager verwaltet</span><span class="sxs-lookup"><span data-stu-id="8c973-130">Managed by Config Manager</span></span>|



