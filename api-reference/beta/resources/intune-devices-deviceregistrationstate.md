---
title: DeviceRegistrationState Enum-Typ
description: Registrierung Gerätestatus.
author: tfitzmac
ms.openlocfilehash: a622613bd4ca5e065c3d9eb0331c05c360c1837c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360543"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="18420-103">DeviceRegistrationState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="18420-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="18420-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="18420-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18420-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="18420-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18420-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="18420-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18420-107">Registrierung Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="18420-107">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="18420-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="18420-108">Members</span></span>
|<span data-ttu-id="18420-109">Member</span><span class="sxs-lookup"><span data-stu-id="18420-109">Member</span></span>|<span data-ttu-id="18420-110">Wert</span><span class="sxs-lookup"><span data-stu-id="18420-110">Value</span></span>|<span data-ttu-id="18420-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="18420-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18420-112">nicht registriert</span><span class="sxs-lookup"><span data-stu-id="18420-112">notRegistered</span></span>|<span data-ttu-id="18420-113">0</span><span class="sxs-lookup"><span data-stu-id="18420-113">0</span></span>|<span data-ttu-id="18420-114">Das Gerät ist nicht registriert.</span><span class="sxs-lookup"><span data-stu-id="18420-114">The device is not registered.</span></span>|
|<span data-ttu-id="18420-115">registriert</span><span class="sxs-lookup"><span data-stu-id="18420-115">registered</span></span>|<span data-ttu-id="18420-116">2</span><span class="sxs-lookup"><span data-stu-id="18420-116">2</span></span>|<span data-ttu-id="18420-117">Das Gerät registriert ist.</span><span class="sxs-lookup"><span data-stu-id="18420-117">The device is registered.</span></span>|
|<span data-ttu-id="18420-118">widerrufen</span><span class="sxs-lookup"><span data-stu-id="18420-118">revoked</span></span>|<span data-ttu-id="18420-119">3</span><span class="sxs-lookup"><span data-stu-id="18420-119">3</span></span>|<span data-ttu-id="18420-120">Das Gerät wurde blockiert, gelöscht oder zurückgezogen.</span><span class="sxs-lookup"><span data-stu-id="18420-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="18420-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="18420-121">keyConflict</span></span>|<span data-ttu-id="18420-122">4</span><span class="sxs-lookup"><span data-stu-id="18420-122">4</span></span>|<span data-ttu-id="18420-123">Das Gerät hat einen Konflikt mit Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="18420-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="18420-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="18420-124">approvalPending</span></span>|<span data-ttu-id="18420-125">5</span><span class="sxs-lookup"><span data-stu-id="18420-125">5</span></span>|<span data-ttu-id="18420-126">Das Gerät ist ausstehender Genehmigung.</span><span class="sxs-lookup"><span data-stu-id="18420-126">The device is pending approval.</span></span>|
|<span data-ttu-id="18420-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="18420-127">certificateReset</span></span>|<span data-ttu-id="18420-128">6</span><span class="sxs-lookup"><span data-stu-id="18420-128">6</span></span>|<span data-ttu-id="18420-129">Das Gerät Zertifikat wurde zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="18420-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="18420-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="18420-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="18420-131">7</span><span class="sxs-lookup"><span data-stu-id="18420-131">7</span></span>|<span data-ttu-id="18420-132">Das Gerät ist nicht registriert und ausstehenden Registrierung.</span><span class="sxs-lookup"><span data-stu-id="18420-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="18420-133">unknown</span><span class="sxs-lookup"><span data-stu-id="18420-133">unknown</span></span>|<span data-ttu-id="18420-134">8</span><span class="sxs-lookup"><span data-stu-id="18420-134">8</span></span>|<span data-ttu-id="18420-135">Die Registrierung Gerätestatus ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="18420-135">The device registration status is unknown.</span></span>|





