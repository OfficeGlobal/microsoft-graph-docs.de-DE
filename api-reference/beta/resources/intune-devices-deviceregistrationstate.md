---
title: deviceRegistrationState-Enumerationstyp
description: Status der Geräteregistrierung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f04d8c0fddb966504675e3b4c677dfd0bbabe64c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144625"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="a8355-103">deviceRegistrationState-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="a8355-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="a8355-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8355-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8355-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a8355-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8355-106">Status der Geräteregistrierung.</span><span class="sxs-lookup"><span data-stu-id="a8355-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="a8355-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="a8355-107">Members</span></span>
|<span data-ttu-id="a8355-108">Element</span><span class="sxs-lookup"><span data-stu-id="a8355-108">Member</span></span>|<span data-ttu-id="a8355-109">Wert</span><span class="sxs-lookup"><span data-stu-id="a8355-109">Value</span></span>|<span data-ttu-id="a8355-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8355-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8355-111">notRegistered</span><span class="sxs-lookup"><span data-stu-id="a8355-111">notRegistered</span></span>|<span data-ttu-id="a8355-112">0</span><span class="sxs-lookup"><span data-stu-id="a8355-112">0</span></span>|<span data-ttu-id="a8355-113">Das Gerät ist nicht registriert.</span><span class="sxs-lookup"><span data-stu-id="a8355-113">The device is not registered.</span></span>|
|<span data-ttu-id="a8355-114">registriert</span><span class="sxs-lookup"><span data-stu-id="a8355-114">registered</span></span>|<span data-ttu-id="a8355-115">2</span><span class="sxs-lookup"><span data-stu-id="a8355-115">2</span></span>|<span data-ttu-id="a8355-116">Das Gerät ist registriert.</span><span class="sxs-lookup"><span data-stu-id="a8355-116">The device is registered.</span></span>|
|<span data-ttu-id="a8355-117">gesperrt</span><span class="sxs-lookup"><span data-stu-id="a8355-117">revoked</span></span>|<span data-ttu-id="a8355-118">3</span><span class="sxs-lookup"><span data-stu-id="a8355-118">3</span></span>|<span data-ttu-id="a8355-119">Das Gerät wurde gesperrt, gelöscht oder im Ruhestand.</span><span class="sxs-lookup"><span data-stu-id="a8355-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="a8355-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="a8355-120">keyConflict</span></span>|<span data-ttu-id="a8355-121">4</span><span class="sxs-lookup"><span data-stu-id="a8355-121">4</span></span>|<span data-ttu-id="a8355-122">Das Gerät hat einen Schlüsselkonflikt.</span><span class="sxs-lookup"><span data-stu-id="a8355-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="a8355-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="a8355-123">approvalPending</span></span>|<span data-ttu-id="a8355-124">5</span><span class="sxs-lookup"><span data-stu-id="a8355-124">5</span></span>|<span data-ttu-id="a8355-125">Das Gerät steht zur Genehmigung.</span><span class="sxs-lookup"><span data-stu-id="a8355-125">The device is pending approval.</span></span>|
|<span data-ttu-id="a8355-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="a8355-126">certificateReset</span></span>|<span data-ttu-id="a8355-127">6</span><span class="sxs-lookup"><span data-stu-id="a8355-127">6</span></span>|<span data-ttu-id="a8355-128">Das Gerätezertifikat wurde zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="a8355-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="a8355-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="a8355-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="a8355-130">7</span><span class="sxs-lookup"><span data-stu-id="a8355-130">7</span></span>|<span data-ttu-id="a8355-131">Das Gerät ist nicht registriert und steht noch aus der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="a8355-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="a8355-132">unknown</span><span class="sxs-lookup"><span data-stu-id="a8355-132">unknown</span></span>|<span data-ttu-id="a8355-133">8</span><span class="sxs-lookup"><span data-stu-id="a8355-133">8</span></span>|<span data-ttu-id="a8355-134">Der Geräte Registrierungsstatus ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="a8355-134">The device registration status is unknown.</span></span>|




