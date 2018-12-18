---
title: DeviceRegistrationState Enum-Typ
description: Registrierung Gerätestatus.
author: tfitzmac
ms.openlocfilehash: 9fdd5cd3a63472e841f0d97f8cbee3a0f548380d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320090"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="84f9f-103">DeviceRegistrationState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="84f9f-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="84f9f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="84f9f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84f9f-105">Registrierung Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="84f9f-105">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="84f9f-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="84f9f-106">Members</span></span>
|<span data-ttu-id="84f9f-107">Member</span><span class="sxs-lookup"><span data-stu-id="84f9f-107">Member</span></span>|<span data-ttu-id="84f9f-108">Wert</span><span class="sxs-lookup"><span data-stu-id="84f9f-108">Value</span></span>|<span data-ttu-id="84f9f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84f9f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84f9f-110">nicht registriert</span><span class="sxs-lookup"><span data-stu-id="84f9f-110">notRegistered</span></span>|<span data-ttu-id="84f9f-111">0</span><span class="sxs-lookup"><span data-stu-id="84f9f-111">0</span></span>|<span data-ttu-id="84f9f-112">Das Gerät ist nicht registriert.</span><span class="sxs-lookup"><span data-stu-id="84f9f-112">The device is not registered.</span></span>|
|<span data-ttu-id="84f9f-113">registriert</span><span class="sxs-lookup"><span data-stu-id="84f9f-113">registered</span></span>|<span data-ttu-id="84f9f-114">2</span><span class="sxs-lookup"><span data-stu-id="84f9f-114">2</span></span>|<span data-ttu-id="84f9f-115">Das Gerät registriert ist.</span><span class="sxs-lookup"><span data-stu-id="84f9f-115">The device is registered.</span></span>|
|<span data-ttu-id="84f9f-116">widerrufen</span><span class="sxs-lookup"><span data-stu-id="84f9f-116">revoked</span></span>|<span data-ttu-id="84f9f-117">3</span><span class="sxs-lookup"><span data-stu-id="84f9f-117">3</span></span>|<span data-ttu-id="84f9f-118">Das Gerät wurde blockiert, gelöscht oder zurückgezogen.</span><span class="sxs-lookup"><span data-stu-id="84f9f-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="84f9f-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="84f9f-119">keyConflict</span></span>|<span data-ttu-id="84f9f-120">4</span><span class="sxs-lookup"><span data-stu-id="84f9f-120">4</span></span>|<span data-ttu-id="84f9f-121">Das Gerät hat einen Konflikt mit Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="84f9f-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="84f9f-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="84f9f-122">approvalPending</span></span>|<span data-ttu-id="84f9f-123">5</span><span class="sxs-lookup"><span data-stu-id="84f9f-123">5</span></span>|<span data-ttu-id="84f9f-124">Das Gerät ist ausstehender Genehmigung.</span><span class="sxs-lookup"><span data-stu-id="84f9f-124">The device is pending approval.</span></span>|
|<span data-ttu-id="84f9f-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="84f9f-125">certificateReset</span></span>|<span data-ttu-id="84f9f-126">6</span><span class="sxs-lookup"><span data-stu-id="84f9f-126">6</span></span>|<span data-ttu-id="84f9f-127">Das Gerät Zertifikat wurde zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="84f9f-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="84f9f-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="84f9f-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="84f9f-129">7</span><span class="sxs-lookup"><span data-stu-id="84f9f-129">7</span></span>|<span data-ttu-id="84f9f-130">Das Gerät ist nicht registriert und ausstehenden Registrierung.</span><span class="sxs-lookup"><span data-stu-id="84f9f-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="84f9f-131">unknown</span><span class="sxs-lookup"><span data-stu-id="84f9f-131">unknown</span></span>|<span data-ttu-id="84f9f-132">8</span><span class="sxs-lookup"><span data-stu-id="84f9f-132">8</span></span>|<span data-ttu-id="84f9f-133">Die Registrierung Gerätestatus ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="84f9f-133">The device registration status is unknown.</span></span>|



