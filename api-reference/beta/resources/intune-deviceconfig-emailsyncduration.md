---
title: emailSyncDuration-Enumerationstyp
description: Mögliche Werte für die e-Mail-Synchronisierungsdauer.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f2408150ea590a5d154b71521ca46df7c0fcff9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142266"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="a22d1-103">emailSyncDuration-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="a22d1-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="a22d1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a22d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a22d1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a22d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a22d1-106">Mögliche Werte für die e-Mail-Synchronisierungsdauer.</span><span class="sxs-lookup"><span data-stu-id="a22d1-106">Possible values for email sync duration.</span></span>

## <a name="members"></a><span data-ttu-id="a22d1-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="a22d1-107">Members</span></span>
|<span data-ttu-id="a22d1-108">Element</span><span class="sxs-lookup"><span data-stu-id="a22d1-108">Member</span></span>|<span data-ttu-id="a22d1-109">Wert</span><span class="sxs-lookup"><span data-stu-id="a22d1-109">Value</span></span>|<span data-ttu-id="a22d1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a22d1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a22d1-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="a22d1-111">userDefined</span></span>|<span data-ttu-id="a22d1-112">0</span><span class="sxs-lookup"><span data-stu-id="a22d1-112">0</span></span>|<span data-ttu-id="a22d1-113">Benutzerdefiniert, Standardwert, keine Absicht.</span><span class="sxs-lookup"><span data-stu-id="a22d1-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="a22d1-114">oneDay</span><span class="sxs-lookup"><span data-stu-id="a22d1-114">oneDay</span></span>|<span data-ttu-id="a22d1-115">1</span><span class="sxs-lookup"><span data-stu-id="a22d1-115">1</span></span>|<span data-ttu-id="a22d1-116">Synchronisieren eines Tages der e-Mail.</span><span class="sxs-lookup"><span data-stu-id="a22d1-116">Sync one day of email.</span></span>|
|<span data-ttu-id="a22d1-117">threeDays</span><span class="sxs-lookup"><span data-stu-id="a22d1-117">threeDays</span></span>|<span data-ttu-id="a22d1-118">2</span><span class="sxs-lookup"><span data-stu-id="a22d1-118">2</span></span>|<span data-ttu-id="a22d1-119">Synchronisieren Sie drei Tage e-Mail.</span><span class="sxs-lookup"><span data-stu-id="a22d1-119">Sync three days of email.</span></span>|
|<span data-ttu-id="a22d1-120">oneWeek</span><span class="sxs-lookup"><span data-stu-id="a22d1-120">oneWeek</span></span>|<span data-ttu-id="a22d1-121">3</span><span class="sxs-lookup"><span data-stu-id="a22d1-121">3</span></span>|<span data-ttu-id="a22d1-122">Eine Woche e-Mails synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="a22d1-122">Sync one week of email.</span></span>|
|<span data-ttu-id="a22d1-123">twoweeks starten</span><span class="sxs-lookup"><span data-stu-id="a22d1-123">twoWeeks</span></span>|<span data-ttu-id="a22d1-124">4</span><span class="sxs-lookup"><span data-stu-id="a22d1-124">4</span></span>|<span data-ttu-id="a22d1-125">Zwei Wochen e-Mails synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="a22d1-125">Sync two weeks of email.</span></span>|
|<span data-ttu-id="a22d1-126">Maßgebend Frist</span><span class="sxs-lookup"><span data-stu-id="a22d1-126">oneMonth</span></span>|<span data-ttu-id="a22d1-127">5</span><span class="sxs-lookup"><span data-stu-id="a22d1-127">5</span></span>|<span data-ttu-id="a22d1-128">Einen Monat e-Mails synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="a22d1-128">Sync one month of email.</span></span>|
|<span data-ttu-id="a22d1-129">Unlimited</span><span class="sxs-lookup"><span data-stu-id="a22d1-129">unlimited</span></span>|<span data-ttu-id="a22d1-130">6</span><span class="sxs-lookup"><span data-stu-id="a22d1-130">6</span></span>|<span data-ttu-id="a22d1-131">Synchronisieren einer unbegrenzten Dauer von e-Mails.</span><span class="sxs-lookup"><span data-stu-id="a22d1-131">Sync an unlimited duration of email.</span></span>|




