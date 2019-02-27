---
title: complianceState-Enumerationstyp
description: Konformitätsstatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d578417c616fc2dbf30b8fe95d2f58ede5fd3df2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253358"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="90969-103">complianceState-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="90969-103">complianceState enum type</span></span>

> <span data-ttu-id="90969-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="90969-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90969-105">Konformitätsstatus.</span><span class="sxs-lookup"><span data-stu-id="90969-105">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="90969-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="90969-106">Members</span></span>
|<span data-ttu-id="90969-107">Element</span><span class="sxs-lookup"><span data-stu-id="90969-107">Member</span></span>|<span data-ttu-id="90969-108">Wert</span><span class="sxs-lookup"><span data-stu-id="90969-108">Value</span></span>|<span data-ttu-id="90969-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="90969-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90969-110">unknown</span><span class="sxs-lookup"><span data-stu-id="90969-110">unknown</span></span>|<span data-ttu-id="90969-111">0</span><span class="sxs-lookup"><span data-stu-id="90969-111">0</span></span>|<span data-ttu-id="90969-112">Unbekannt.</span><span class="sxs-lookup"><span data-stu-id="90969-112">Unknown.</span></span>|
|<span data-ttu-id="90969-113">kompatibel</span><span class="sxs-lookup"><span data-stu-id="90969-113">compliant</span></span>|<span data-ttu-id="90969-114">1</span><span class="sxs-lookup"><span data-stu-id="90969-114">1</span></span>|<span data-ttu-id="90969-115">Kompatibel.</span><span class="sxs-lookup"><span data-stu-id="90969-115">Compliant.</span></span>|
|<span data-ttu-id="90969-116">konform</span><span class="sxs-lookup"><span data-stu-id="90969-116">noncompliant</span></span>|<span data-ttu-id="90969-117">2</span><span class="sxs-lookup"><span data-stu-id="90969-117">2</span></span>|<span data-ttu-id="90969-118">Das Gerät ist nicht kompatibel und wird von Unternehmensressourcen blockiert.</span><span class="sxs-lookup"><span data-stu-id="90969-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="90969-119">Konflikt</span><span class="sxs-lookup"><span data-stu-id="90969-119">conflict</span></span>|<span data-ttu-id="90969-120">3</span><span class="sxs-lookup"><span data-stu-id="90969-120">3</span></span>|<span data-ttu-id="90969-121">Konflikt mit anderen Regeln.</span><span class="sxs-lookup"><span data-stu-id="90969-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="90969-122">error</span><span class="sxs-lookup"><span data-stu-id="90969-122">error</span></span>|<span data-ttu-id="90969-123">4</span><span class="sxs-lookup"><span data-stu-id="90969-123">4</span></span>|<span data-ttu-id="90969-124">Fehler</span><span class="sxs-lookup"><span data-stu-id="90969-124">Error.</span></span>|
|<span data-ttu-id="90969-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="90969-125">inGracePeriod</span></span>|<span data-ttu-id="90969-126">254</span><span class="sxs-lookup"><span data-stu-id="90969-126">254</span></span>|<span data-ttu-id="90969-127">Das Gerät ist nicht kompatibel, hat jedoch weiterhin Zugriff auf Unternehmensressourcen.</span><span class="sxs-lookup"><span data-stu-id="90969-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="90969-128">configManager</span><span class="sxs-lookup"><span data-stu-id="90969-128">configManager</span></span>|<span data-ttu-id="90969-129">255</span><span class="sxs-lookup"><span data-stu-id="90969-129">255</span></span>|<span data-ttu-id="90969-130">Verwaltet von config Manager</span><span class="sxs-lookup"><span data-stu-id="90969-130">Managed by Config Manager</span></span>|



