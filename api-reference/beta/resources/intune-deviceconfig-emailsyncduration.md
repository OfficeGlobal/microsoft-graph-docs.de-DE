---
title: EmailSyncDuration Enum-Typ
description: Mögliche Werte für die Dauer der e-Mail-Synchronisierung.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d83a1ceb82820ddc44d8753e8ed05e00de09e36e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819383"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="d6384-103">EmailSyncDuration Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="d6384-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="d6384-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d6384-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6384-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d6384-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6384-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d6384-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6384-107">Mögliche Werte für die Dauer der e-Mail-Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="d6384-107">Possible values for email sync duration.</span></span>
## <a name="members"></a><span data-ttu-id="d6384-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="d6384-108">Members</span></span>
|<span data-ttu-id="d6384-109">Element</span><span class="sxs-lookup"><span data-stu-id="d6384-109">Member</span></span>|<span data-ttu-id="d6384-110">Wert</span><span class="sxs-lookup"><span data-stu-id="d6384-110">Value</span></span>|<span data-ttu-id="d6384-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6384-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6384-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="d6384-112">userDefined</span></span>|<span data-ttu-id="d6384-113">0</span><span class="sxs-lookup"><span data-stu-id="d6384-113">0</span></span>|<span data-ttu-id="d6384-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="d6384-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="d6384-115">oneDay</span><span class="sxs-lookup"><span data-stu-id="d6384-115">oneDay</span></span>|<span data-ttu-id="d6384-116">1</span><span class="sxs-lookup"><span data-stu-id="d6384-116">1</span></span>|<span data-ttu-id="d6384-117">Synchronisieren von e-Mail für einen Tag.</span><span class="sxs-lookup"><span data-stu-id="d6384-117">Sync one day of email.</span></span>|
|<span data-ttu-id="d6384-118">threeDays</span><span class="sxs-lookup"><span data-stu-id="d6384-118">threeDays</span></span>|<span data-ttu-id="d6384-119">2</span><span class="sxs-lookup"><span data-stu-id="d6384-119">2</span></span>|<span data-ttu-id="d6384-120">Synchronisieren Sie drei Tage von e-Mails.</span><span class="sxs-lookup"><span data-stu-id="d6384-120">Sync three days of email.</span></span>|
|<span data-ttu-id="d6384-121">oneWeek</span><span class="sxs-lookup"><span data-stu-id="d6384-121">oneWeek</span></span>|<span data-ttu-id="d6384-122">3</span><span class="sxs-lookup"><span data-stu-id="d6384-122">3</span></span>|<span data-ttu-id="d6384-123">Synchronisieren Sie eine Woche vor e-Mail.</span><span class="sxs-lookup"><span data-stu-id="d6384-123">Sync one week of email.</span></span>|
|<span data-ttu-id="d6384-124">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="d6384-124">twoWeeks</span></span>|<span data-ttu-id="d6384-125">4</span><span class="sxs-lookup"><span data-stu-id="d6384-125">4</span></span>|<span data-ttu-id="d6384-126">Synchronisieren von zwei Wochen von e-Mails.</span><span class="sxs-lookup"><span data-stu-id="d6384-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="d6384-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="d6384-127">oneMonth</span></span>|<span data-ttu-id="d6384-128">5</span><span class="sxs-lookup"><span data-stu-id="d6384-128">5</span></span>|<span data-ttu-id="d6384-129">Synchronisieren eines Monats e-Mail.</span><span class="sxs-lookup"><span data-stu-id="d6384-129">Sync one month of email.</span></span>|
|<span data-ttu-id="d6384-130">unbegrenzt</span><span class="sxs-lookup"><span data-stu-id="d6384-130">unlimited</span></span>|<span data-ttu-id="d6384-131">6</span><span class="sxs-lookup"><span data-stu-id="d6384-131">6</span></span>|<span data-ttu-id="d6384-132">Synchronisieren Sie eine unbegrenzte Dauer von e-Mail.</span><span class="sxs-lookup"><span data-stu-id="d6384-132">Sync an unlimited duration of email.</span></span>|





