---
title: deviceRegistrationState-Enumerationstyp
description: Status der Geräteregistrierung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b3bee7ab56f07dd6f27c20c771329ba84edbb19
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264134"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="e9fcc-103">deviceRegistrationState-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="e9fcc-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="e9fcc-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e9fcc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9fcc-105">Status der Geräteregistrierung.</span><span class="sxs-lookup"><span data-stu-id="e9fcc-105">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="e9fcc-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="e9fcc-106">Members</span></span>
|<span data-ttu-id="e9fcc-107">Element</span><span class="sxs-lookup"><span data-stu-id="e9fcc-107">Member</span></span>|<span data-ttu-id="e9fcc-108">Wert</span><span class="sxs-lookup"><span data-stu-id="e9fcc-108">Value</span></span>|<span data-ttu-id="e9fcc-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e9fcc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9fcc-110">notRegistered</span><span class="sxs-lookup"><span data-stu-id="e9fcc-110">notRegistered</span></span>|<span data-ttu-id="e9fcc-111">0</span><span class="sxs-lookup"><span data-stu-id="e9fcc-111">0</span></span>|<span data-ttu-id="e9fcc-112">Das Gerät ist nicht registriert.</span><span class="sxs-lookup"><span data-stu-id="e9fcc-112">The device is not registered.</span></span>|
|<span data-ttu-id="e9fcc-113">registriert</span><span class="sxs-lookup"><span data-stu-id="e9fcc-113">registered</span></span>|<span data-ttu-id="e9fcc-114">2</span><span class="sxs-lookup"><span data-stu-id="e9fcc-114">2</span></span>|<span data-ttu-id="e9fcc-115">Das Gerät ist registriert.</span><span class="sxs-lookup"><span data-stu-id="e9fcc-115">The device is registered.</span></span>|
|<span data-ttu-id="e9fcc-116">gesperrt</span><span class="sxs-lookup"><span data-stu-id="e9fcc-116">revoked</span></span>|<span data-ttu-id="e9fcc-117">3</span><span class="sxs-lookup"><span data-stu-id="e9fcc-117">3</span></span>|<span data-ttu-id="e9fcc-118">Das Gerät wurde gesperrt, gelöscht oder im Ruhestand.</span><span class="sxs-lookup"><span data-stu-id="e9fcc-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="e9fcc-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="e9fcc-119">keyConflict</span></span>|<span data-ttu-id="e9fcc-120">4</span><span class="sxs-lookup"><span data-stu-id="e9fcc-120">4</span></span>|<span data-ttu-id="e9fcc-121">Das Gerät hat einen Schlüsselkonflikt.</span><span class="sxs-lookup"><span data-stu-id="e9fcc-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="e9fcc-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="e9fcc-122">approvalPending</span></span>|<span data-ttu-id="e9fcc-123">5</span><span class="sxs-lookup"><span data-stu-id="e9fcc-123">5</span></span>|<span data-ttu-id="e9fcc-124">Das Gerät steht zur Genehmigung.</span><span class="sxs-lookup"><span data-stu-id="e9fcc-124">The device is pending approval.</span></span>|
|<span data-ttu-id="e9fcc-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="e9fcc-125">certificateReset</span></span>|<span data-ttu-id="e9fcc-126">6</span><span class="sxs-lookup"><span data-stu-id="e9fcc-126">6</span></span>|<span data-ttu-id="e9fcc-127">Das Gerätezertifikat wurde zurückgesetzt.</span><span class="sxs-lookup"><span data-stu-id="e9fcc-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="e9fcc-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="e9fcc-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="e9fcc-129">7</span><span class="sxs-lookup"><span data-stu-id="e9fcc-129">7</span></span>|<span data-ttu-id="e9fcc-130">Das Gerät ist nicht registriert und steht noch aus der Registrierung.</span><span class="sxs-lookup"><span data-stu-id="e9fcc-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="e9fcc-131">unknown</span><span class="sxs-lookup"><span data-stu-id="e9fcc-131">unknown</span></span>|<span data-ttu-id="e9fcc-132">8</span><span class="sxs-lookup"><span data-stu-id="e9fcc-132">8</span></span>|<span data-ttu-id="e9fcc-133">Der Geräte Registrierungsstatus ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="e9fcc-133">The device registration status is unknown.</span></span>|



