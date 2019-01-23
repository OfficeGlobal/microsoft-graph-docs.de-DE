---
title: EmailSyncDuration Enum-Typ
description: Mögliche Werte für die Dauer der e-Mail-Synchronisierung.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8bf62aea1904c0fd25867aef308ca5a269e3ea20
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399409"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="c26d1-103">EmailSyncDuration Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="c26d1-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="c26d1-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c26d1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c26d1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c26d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c26d1-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c26d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c26d1-107">Mögliche Werte für die Dauer der e-Mail-Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="c26d1-107">Possible values for email sync duration.</span></span>

## <a name="members"></a><span data-ttu-id="c26d1-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="c26d1-108">Members</span></span>
|<span data-ttu-id="c26d1-109">Member</span><span class="sxs-lookup"><span data-stu-id="c26d1-109">Member</span></span>|<span data-ttu-id="c26d1-110">Wert</span><span class="sxs-lookup"><span data-stu-id="c26d1-110">Value</span></span>|<span data-ttu-id="c26d1-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c26d1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c26d1-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="c26d1-112">userDefined</span></span>|<span data-ttu-id="c26d1-113">0</span><span class="sxs-lookup"><span data-stu-id="c26d1-113">0</span></span>|<span data-ttu-id="c26d1-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="c26d1-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c26d1-115">oneDay</span><span class="sxs-lookup"><span data-stu-id="c26d1-115">oneDay</span></span>|<span data-ttu-id="c26d1-116">1</span><span class="sxs-lookup"><span data-stu-id="c26d1-116">1</span></span>|<span data-ttu-id="c26d1-117">Synchronisieren von e-Mail für einen Tag.</span><span class="sxs-lookup"><span data-stu-id="c26d1-117">Sync one day of email.</span></span>|
|<span data-ttu-id="c26d1-118">threeDays</span><span class="sxs-lookup"><span data-stu-id="c26d1-118">threeDays</span></span>|<span data-ttu-id="c26d1-119">2</span><span class="sxs-lookup"><span data-stu-id="c26d1-119">2</span></span>|<span data-ttu-id="c26d1-120">Synchronisieren Sie drei Tage von e-Mails.</span><span class="sxs-lookup"><span data-stu-id="c26d1-120">Sync three days of email.</span></span>|
|<span data-ttu-id="c26d1-121">oneWeek</span><span class="sxs-lookup"><span data-stu-id="c26d1-121">oneWeek</span></span>|<span data-ttu-id="c26d1-122">3</span><span class="sxs-lookup"><span data-stu-id="c26d1-122">3</span></span>|<span data-ttu-id="c26d1-123">Synchronisieren Sie eine Woche vor e-Mail.</span><span class="sxs-lookup"><span data-stu-id="c26d1-123">Sync one week of email.</span></span>|
|<span data-ttu-id="c26d1-124">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="c26d1-124">twoWeeks</span></span>|<span data-ttu-id="c26d1-125">4</span><span class="sxs-lookup"><span data-stu-id="c26d1-125">4</span></span>|<span data-ttu-id="c26d1-126">Synchronisieren von zwei Wochen von e-Mails.</span><span class="sxs-lookup"><span data-stu-id="c26d1-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="c26d1-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="c26d1-127">oneMonth</span></span>|<span data-ttu-id="c26d1-128">5</span><span class="sxs-lookup"><span data-stu-id="c26d1-128">5</span></span>|<span data-ttu-id="c26d1-129">Synchronisieren eines Monats e-Mail.</span><span class="sxs-lookup"><span data-stu-id="c26d1-129">Sync one month of email.</span></span>|
|<span data-ttu-id="c26d1-130">unbegrenzt</span><span class="sxs-lookup"><span data-stu-id="c26d1-130">unlimited</span></span>|<span data-ttu-id="c26d1-131">6</span><span class="sxs-lookup"><span data-stu-id="c26d1-131">6</span></span>|<span data-ttu-id="c26d1-132">Synchronisieren Sie eine unbegrenzte Dauer von e-Mail.</span><span class="sxs-lookup"><span data-stu-id="c26d1-132">Sync an unlimited duration of email.</span></span>|




