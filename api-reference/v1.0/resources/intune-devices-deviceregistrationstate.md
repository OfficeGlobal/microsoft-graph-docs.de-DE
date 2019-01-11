---
title: DeviceRegistrationState Enum-Typ
description: Registrierung Gerätestatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e2b755d213d39beb228afe603b2066b55416f14c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857323"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="e6b1a-103">DeviceRegistrationState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="e6b1a-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="e6b1a-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e6b1a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6b1a-105">Registrierung Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="e6b1a-105">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="e6b1a-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="e6b1a-106">Members</span></span>
|<span data-ttu-id="e6b1a-107">Element</span><span class="sxs-lookup"><span data-stu-id="e6b1a-107">Member</span></span>|<span data-ttu-id="e6b1a-108">Wert</span><span class="sxs-lookup"><span data-stu-id="e6b1a-108">Value</span></span>|<span data-ttu-id="e6b1a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6b1a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6b1a-110">nicht registriert</span><span class="sxs-lookup"><span data-stu-id="e6b1a-110">notRegistered</span></span>|<span data-ttu-id="e6b1a-111">0</span><span class="sxs-lookup"><span data-stu-id="e6b1a-111">0</span></span>|<span data-ttu-id="e6b1a-112">Das Gerät ist nicht registriert.</span><span class="sxs-lookup"><span data-stu-id="e6b1a-112">The device is not registered.</span></span>|
|<span data-ttu-id="e6b1a-113">registriert</span><span class="sxs-lookup"><span data-stu-id="e6b1a-113">registered</span></span>|<span data-ttu-id="e6b1a-114">2</span><span class="sxs-lookup"><span data-stu-id="e6b1a-114">2</span></span>|<span data-ttu-id="e6b1a-115">Das Gerät registriert ist.</span><span class="sxs-lookup"><span data-stu-id="e6b1a-115">The device is registered.</span></span>|
|<span data-ttu-id="e6b1a-116">widerrufen</span><span class="sxs-lookup"><span data-stu-id="e6b1a-116">revoked</span></span>|<span data-ttu-id="e6b1a-117">3</span><span class="sxs-lookup"><span data-stu-id="e6b1a-117">3</span></span>|<span data-ttu-id="e6b1a-118">Das Gerät wurde blockiert, gelöscht oder zurückgezogen.</span><span class="sxs-lookup"><span data-stu-id="e6b1a-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="e6b1a-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="e6b1a-119">keyConflict</span></span>|<span data-ttu-id="e6b1a-120">4</span><span class="sxs-lookup"><span data-stu-id="e6b1a-120">4</span></span>|<span data-ttu-id="e6b1a-121">Das Gerät hat einen Konflikt mit Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="e6b1a-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="e6b1a-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="e6b1a-122">approvalPending</span></span>|<span data-ttu-id="e6b1a-123">5</span><span class="sxs-lookup"><span data-stu-id="e6b1a-123">5</span></span>|<span data-ttu-id="e6b1a-124">Das Gerät ist ausstehender Genehmigung.</span><span class="sxs-lookup"><span data-stu-id="e6b1a-124">The device is pending approval.</span></span>|
|<span data-ttu-id="e6b1a-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="e6b1a-125">certificateReset</span></span>|<span data-ttu-id="e6b1a-126">6</span><span class="sxs-lookup"><span data-stu-id="e6b1a-126">6</span></span>|<span data-ttu-id="e6b1a-127">Das Gerät Zertifikat wurde zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="e6b1a-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="e6b1a-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="e6b1a-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="e6b1a-129">7</span><span class="sxs-lookup"><span data-stu-id="e6b1a-129">7</span></span>|<span data-ttu-id="e6b1a-130">Das Gerät ist nicht registriert und ausstehenden Registrierung.</span><span class="sxs-lookup"><span data-stu-id="e6b1a-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="e6b1a-131">unknown</span><span class="sxs-lookup"><span data-stu-id="e6b1a-131">unknown</span></span>|<span data-ttu-id="e6b1a-132">8</span><span class="sxs-lookup"><span data-stu-id="e6b1a-132">8</span></span>|<span data-ttu-id="e6b1a-133">Die Registrierung Gerätestatus ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="e6b1a-133">The device registration status is unknown.</span></span>|



