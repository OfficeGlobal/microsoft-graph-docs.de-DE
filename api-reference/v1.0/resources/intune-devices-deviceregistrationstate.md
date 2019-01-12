---
title: DeviceRegistrationState Enum-Typ
description: Registrierung Gerätestatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5b0048385930166de3329ef9d407f5ddd19efc77
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911896"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="99882-103">DeviceRegistrationState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="99882-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="99882-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="99882-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99882-105">Registrierung Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="99882-105">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="99882-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="99882-106">Members</span></span>
|<span data-ttu-id="99882-107">Element</span><span class="sxs-lookup"><span data-stu-id="99882-107">Member</span></span>|<span data-ttu-id="99882-108">Wert</span><span class="sxs-lookup"><span data-stu-id="99882-108">Value</span></span>|<span data-ttu-id="99882-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99882-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99882-110">nicht registriert</span><span class="sxs-lookup"><span data-stu-id="99882-110">notRegistered</span></span>|<span data-ttu-id="99882-111">0</span><span class="sxs-lookup"><span data-stu-id="99882-111">0</span></span>|<span data-ttu-id="99882-112">Das Gerät ist nicht registriert.</span><span class="sxs-lookup"><span data-stu-id="99882-112">The device is not registered.</span></span>|
|<span data-ttu-id="99882-113">registriert</span><span class="sxs-lookup"><span data-stu-id="99882-113">registered</span></span>|<span data-ttu-id="99882-114">2</span><span class="sxs-lookup"><span data-stu-id="99882-114">2</span></span>|<span data-ttu-id="99882-115">Das Gerät registriert ist.</span><span class="sxs-lookup"><span data-stu-id="99882-115">The device is registered.</span></span>|
|<span data-ttu-id="99882-116">widerrufen</span><span class="sxs-lookup"><span data-stu-id="99882-116">revoked</span></span>|<span data-ttu-id="99882-117">3</span><span class="sxs-lookup"><span data-stu-id="99882-117">3</span></span>|<span data-ttu-id="99882-118">Das Gerät wurde blockiert, gelöscht oder zurückgezogen.</span><span class="sxs-lookup"><span data-stu-id="99882-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="99882-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="99882-119">keyConflict</span></span>|<span data-ttu-id="99882-120">4</span><span class="sxs-lookup"><span data-stu-id="99882-120">4</span></span>|<span data-ttu-id="99882-121">Das Gerät hat einen Konflikt mit Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="99882-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="99882-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="99882-122">approvalPending</span></span>|<span data-ttu-id="99882-123">5</span><span class="sxs-lookup"><span data-stu-id="99882-123">5</span></span>|<span data-ttu-id="99882-124">Das Gerät ist ausstehender Genehmigung.</span><span class="sxs-lookup"><span data-stu-id="99882-124">The device is pending approval.</span></span>|
|<span data-ttu-id="99882-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="99882-125">certificateReset</span></span>|<span data-ttu-id="99882-126">6</span><span class="sxs-lookup"><span data-stu-id="99882-126">6</span></span>|<span data-ttu-id="99882-127">Das Gerät Zertifikat wurde zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="99882-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="99882-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="99882-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="99882-129">7</span><span class="sxs-lookup"><span data-stu-id="99882-129">7</span></span>|<span data-ttu-id="99882-130">Das Gerät ist nicht registriert und ausstehenden Registrierung.</span><span class="sxs-lookup"><span data-stu-id="99882-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="99882-131">unknown</span><span class="sxs-lookup"><span data-stu-id="99882-131">unknown</span></span>|<span data-ttu-id="99882-132">8</span><span class="sxs-lookup"><span data-stu-id="99882-132">8</span></span>|<span data-ttu-id="99882-133">Die Registrierung Gerätestatus ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="99882-133">The device registration status is unknown.</span></span>|



