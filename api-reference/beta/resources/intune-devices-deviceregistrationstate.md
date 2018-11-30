---
title: DeviceRegistrationState Enum-Typ
description: Registrierung Gerätestatus.
ms.openlocfilehash: 5496bce53e061894a829745fce0687815c855c01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065113"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="d432a-103">DeviceRegistrationState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="d432a-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="d432a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d432a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d432a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d432a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d432a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d432a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d432a-107">Registrierung Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="d432a-107">Device registration status.</span></span>
## <a name="members"></a><span data-ttu-id="d432a-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="d432a-108">Members</span></span>
|<span data-ttu-id="d432a-109">Element</span><span class="sxs-lookup"><span data-stu-id="d432a-109">Member</span></span>|<span data-ttu-id="d432a-110">Wert</span><span class="sxs-lookup"><span data-stu-id="d432a-110">Value</span></span>|<span data-ttu-id="d432a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d432a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d432a-112">nicht registriert</span><span class="sxs-lookup"><span data-stu-id="d432a-112">notRegistered</span></span>|<span data-ttu-id="d432a-113">0</span><span class="sxs-lookup"><span data-stu-id="d432a-113">0</span></span>|<span data-ttu-id="d432a-114">Das Gerät ist nicht registriert.</span><span class="sxs-lookup"><span data-stu-id="d432a-114">The device is not registered.</span></span>|
|<span data-ttu-id="d432a-115">registriert</span><span class="sxs-lookup"><span data-stu-id="d432a-115">registered</span></span>|<span data-ttu-id="d432a-116">2</span><span class="sxs-lookup"><span data-stu-id="d432a-116">2</span></span>|<span data-ttu-id="d432a-117">Das Gerät registriert ist.</span><span class="sxs-lookup"><span data-stu-id="d432a-117">The device is registered.</span></span>|
|<span data-ttu-id="d432a-118">widerrufen</span><span class="sxs-lookup"><span data-stu-id="d432a-118">revoked</span></span>|<span data-ttu-id="d432a-119">3</span><span class="sxs-lookup"><span data-stu-id="d432a-119">3</span></span>|<span data-ttu-id="d432a-120">Das Gerät wurde blockiert, gelöscht oder zurückgezogen.</span><span class="sxs-lookup"><span data-stu-id="d432a-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="d432a-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="d432a-121">keyConflict</span></span>|<span data-ttu-id="d432a-122">4</span><span class="sxs-lookup"><span data-stu-id="d432a-122">4</span></span>|<span data-ttu-id="d432a-123">Das Gerät hat einen Konflikt mit Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="d432a-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="d432a-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="d432a-124">approvalPending</span></span>|<span data-ttu-id="d432a-125">5</span><span class="sxs-lookup"><span data-stu-id="d432a-125">5</span></span>|<span data-ttu-id="d432a-126">Das Gerät ist ausstehender Genehmigung.</span><span class="sxs-lookup"><span data-stu-id="d432a-126">The device is pending approval.</span></span>|
|<span data-ttu-id="d432a-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="d432a-127">certificateReset</span></span>|<span data-ttu-id="d432a-128">6</span><span class="sxs-lookup"><span data-stu-id="d432a-128">6</span></span>|<span data-ttu-id="d432a-129">Das Gerät Zertifikat wurde zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="d432a-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="d432a-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="d432a-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="d432a-131">7</span><span class="sxs-lookup"><span data-stu-id="d432a-131">7</span></span>|<span data-ttu-id="d432a-132">Das Gerät ist nicht registriert und ausstehenden Registrierung.</span><span class="sxs-lookup"><span data-stu-id="d432a-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="d432a-133">unknown</span><span class="sxs-lookup"><span data-stu-id="d432a-133">unknown</span></span>|<span data-ttu-id="d432a-134">8</span><span class="sxs-lookup"><span data-stu-id="d432a-134">8</span></span>|<span data-ttu-id="d432a-135">Die Registrierung Gerätestatus ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="d432a-135">The device registration status is unknown.</span></span>|





