---
title: DeviceRegistrationState Enum-Typ
description: Registrierung Gerätestatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 90f2dc7f8c11940fa01047d8c61f23c8f0389ed8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396756"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="a1c84-103">DeviceRegistrationState Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="a1c84-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="a1c84-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a1c84-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a1c84-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1c84-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1c84-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a1c84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1c84-107">Registrierung Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="a1c84-107">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="a1c84-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="a1c84-108">Members</span></span>
|<span data-ttu-id="a1c84-109">Member</span><span class="sxs-lookup"><span data-stu-id="a1c84-109">Member</span></span>|<span data-ttu-id="a1c84-110">Wert</span><span class="sxs-lookup"><span data-stu-id="a1c84-110">Value</span></span>|<span data-ttu-id="a1c84-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1c84-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1c84-112">nicht registriert</span><span class="sxs-lookup"><span data-stu-id="a1c84-112">notRegistered</span></span>|<span data-ttu-id="a1c84-113">0</span><span class="sxs-lookup"><span data-stu-id="a1c84-113">0</span></span>|<span data-ttu-id="a1c84-114">Das Gerät ist nicht registriert.</span><span class="sxs-lookup"><span data-stu-id="a1c84-114">The device is not registered.</span></span>|
|<span data-ttu-id="a1c84-115">registriert</span><span class="sxs-lookup"><span data-stu-id="a1c84-115">registered</span></span>|<span data-ttu-id="a1c84-116">2</span><span class="sxs-lookup"><span data-stu-id="a1c84-116">2</span></span>|<span data-ttu-id="a1c84-117">Das Gerät registriert ist.</span><span class="sxs-lookup"><span data-stu-id="a1c84-117">The device is registered.</span></span>|
|<span data-ttu-id="a1c84-118">widerrufen</span><span class="sxs-lookup"><span data-stu-id="a1c84-118">revoked</span></span>|<span data-ttu-id="a1c84-119">3</span><span class="sxs-lookup"><span data-stu-id="a1c84-119">3</span></span>|<span data-ttu-id="a1c84-120">Das Gerät wurde blockiert, gelöscht oder zurückgezogen.</span><span class="sxs-lookup"><span data-stu-id="a1c84-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="a1c84-121">keyConflict</span><span class="sxs-lookup"><span data-stu-id="a1c84-121">keyConflict</span></span>|<span data-ttu-id="a1c84-122">4</span><span class="sxs-lookup"><span data-stu-id="a1c84-122">4</span></span>|<span data-ttu-id="a1c84-123">Das Gerät hat einen Konflikt mit Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="a1c84-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="a1c84-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="a1c84-124">approvalPending</span></span>|<span data-ttu-id="a1c84-125">5</span><span class="sxs-lookup"><span data-stu-id="a1c84-125">5</span></span>|<span data-ttu-id="a1c84-126">Das Gerät ist ausstehender Genehmigung.</span><span class="sxs-lookup"><span data-stu-id="a1c84-126">The device is pending approval.</span></span>|
|<span data-ttu-id="a1c84-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="a1c84-127">certificateReset</span></span>|<span data-ttu-id="a1c84-128">6</span><span class="sxs-lookup"><span data-stu-id="a1c84-128">6</span></span>|<span data-ttu-id="a1c84-129">Das Gerät Zertifikat wurde zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="a1c84-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="a1c84-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="a1c84-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="a1c84-131">7</span><span class="sxs-lookup"><span data-stu-id="a1c84-131">7</span></span>|<span data-ttu-id="a1c84-132">Das Gerät ist nicht registriert und ausstehenden Registrierung.</span><span class="sxs-lookup"><span data-stu-id="a1c84-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="a1c84-133">unknown</span><span class="sxs-lookup"><span data-stu-id="a1c84-133">unknown</span></span>|<span data-ttu-id="a1c84-134">8</span><span class="sxs-lookup"><span data-stu-id="a1c84-134">8</span></span>|<span data-ttu-id="a1c84-135">Die Registrierung Gerätestatus ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="a1c84-135">The device registration status is unknown.</span></span>|




