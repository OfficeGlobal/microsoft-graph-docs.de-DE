---
title: EmailSyncSchedule Enum-Typ
description: Mögliche Werte für e-Mail-Synchronisierungszeitplan.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8285b9a34e208b86b7c53c38e6aa015fd8c37560
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425183"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="f752c-103">EmailSyncSchedule Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="f752c-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="f752c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f752c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f752c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f752c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f752c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f752c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f752c-107">Mögliche Werte für e-Mail-Synchronisierungszeitplan.</span><span class="sxs-lookup"><span data-stu-id="f752c-107">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="f752c-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="f752c-108">Members</span></span>
|<span data-ttu-id="f752c-109">Member</span><span class="sxs-lookup"><span data-stu-id="f752c-109">Member</span></span>|<span data-ttu-id="f752c-110">Wert</span><span class="sxs-lookup"><span data-stu-id="f752c-110">Value</span></span>|<span data-ttu-id="f752c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f752c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f752c-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="f752c-112">userDefined</span></span>|<span data-ttu-id="f752c-113">0</span><span class="sxs-lookup"><span data-stu-id="f752c-113">0</span></span>|<span data-ttu-id="f752c-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="f752c-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="f752c-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="f752c-115">asMessagesArrive</span></span>|<span data-ttu-id="f752c-116">1</span><span class="sxs-lookup"><span data-stu-id="f752c-116">1</span></span>|<span data-ttu-id="f752c-117">Synchronisieren Sie wie Nachrichten eingehen.</span><span class="sxs-lookup"><span data-stu-id="f752c-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="f752c-118">Manuell</span><span class="sxs-lookup"><span data-stu-id="f752c-118">manual</span></span>|<span data-ttu-id="f752c-119">2</span><span class="sxs-lookup"><span data-stu-id="f752c-119">2</span></span>|<span data-ttu-id="f752c-120">Manuell synchronisieren.</span><span class="sxs-lookup"><span data-stu-id="f752c-120">Sync manually.</span></span>|
|<span data-ttu-id="f752c-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="f752c-121">fifteenMinutes</span></span>|<span data-ttu-id="f752c-122">3</span><span class="sxs-lookup"><span data-stu-id="f752c-122">3</span></span>|<span data-ttu-id="f752c-123">Synchronisieren Sie alle 15 Minuten.</span><span class="sxs-lookup"><span data-stu-id="f752c-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="f752c-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="f752c-124">thirtyMinutes</span></span>|<span data-ttu-id="f752c-125">4</span><span class="sxs-lookup"><span data-stu-id="f752c-125">4</span></span>|<span data-ttu-id="f752c-126">Sync alle 30 Minuten.</span><span class="sxs-lookup"><span data-stu-id="f752c-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="f752c-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="f752c-127">sixtyMinutes</span></span>|<span data-ttu-id="f752c-128">5</span><span class="sxs-lookup"><span data-stu-id="f752c-128">5</span></span>|<span data-ttu-id="f752c-129">Sync alle 60 Minuten.</span><span class="sxs-lookup"><span data-stu-id="f752c-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="f752c-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="f752c-130">basedOnMyUsage</span></span>|<span data-ttu-id="f752c-131">6</span><span class="sxs-lookup"><span data-stu-id="f752c-131">6</span></span>|<span data-ttu-id="f752c-132">Die Synchronisierung basierend auf meine Verwendung.</span><span class="sxs-lookup"><span data-stu-id="f752c-132">Sync based on my usage.</span></span>|




