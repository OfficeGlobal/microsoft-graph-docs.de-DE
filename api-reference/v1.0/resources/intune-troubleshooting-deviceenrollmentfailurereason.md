---
title: deviceEnrollmentFailureReason-Enumerationstyp
description: Kategorien für die Registrierung auf höchster Ebene
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 623030bccfac9e023a0d1df2dff7ea317b503485
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258331"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="3c551-103">deviceEnrollmentFailureReason-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="3c551-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="3c551-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3c551-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c551-105">Kategorien für die Registrierung auf höchster Ebene</span><span class="sxs-lookup"><span data-stu-id="3c551-105">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="3c551-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="3c551-106">Members</span></span>
|<span data-ttu-id="3c551-107">Element</span><span class="sxs-lookup"><span data-stu-id="3c551-107">Member</span></span>|<span data-ttu-id="3c551-108">Wert</span><span class="sxs-lookup"><span data-stu-id="3c551-108">Value</span></span>|<span data-ttu-id="3c551-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3c551-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c551-110">unknown</span><span class="sxs-lookup"><span data-stu-id="3c551-110">unknown</span></span>|<span data-ttu-id="3c551-111">0</span><span class="sxs-lookup"><span data-stu-id="3c551-111">0</span></span>|<span data-ttu-id="3c551-112">Standardwert: der Ausfallgrund ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="3c551-112">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="3c551-113">Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="3c551-113">authentication</span></span>|<span data-ttu-id="3c551-114">1</span><span class="sxs-lookup"><span data-stu-id="3c551-114">1</span></span>|<span data-ttu-id="3c551-115">Authentifizierung fehlgeschlagen</span><span class="sxs-lookup"><span data-stu-id="3c551-115">Authentication failed</span></span>|
|<span data-ttu-id="3c551-116">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3c551-116">authorization</span></span>|<span data-ttu-id="3c551-117">2</span><span class="sxs-lookup"><span data-stu-id="3c551-117">2</span></span>|<span data-ttu-id="3c551-118">Der Anruf wurde authentifiziert, aber nicht zur Registrierung autorisiert.</span><span class="sxs-lookup"><span data-stu-id="3c551-118">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="3c551-119">accountValidation</span><span class="sxs-lookup"><span data-stu-id="3c551-119">accountValidation</span></span>|<span data-ttu-id="3c551-120">3</span><span class="sxs-lookup"><span data-stu-id="3c551-120">3</span></span>|<span data-ttu-id="3c551-121">Fehler beim Überprüfen des Kontos für die Registrierung.</span><span class="sxs-lookup"><span data-stu-id="3c551-121">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="3c551-122">(Konto gesperrt, Registrierung nicht aktiviert)</span><span class="sxs-lookup"><span data-stu-id="3c551-122">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="3c551-123">userValidation</span><span class="sxs-lookup"><span data-stu-id="3c551-123">userValidation</span></span>|<span data-ttu-id="3c551-124">4</span><span class="sxs-lookup"><span data-stu-id="3c551-124">4</span></span>|<span data-ttu-id="3c551-125">Der Benutzer konnte nicht validiert werden.</span><span class="sxs-lookup"><span data-stu-id="3c551-125">User could not be validated.</span></span> <span data-ttu-id="3c551-126">(Benutzer ist nicht vorhanden, fehlende Lizenz)</span><span class="sxs-lookup"><span data-stu-id="3c551-126">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="3c551-127">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="3c551-127">deviceNotSupported</span></span>|<span data-ttu-id="3c551-128">5</span><span class="sxs-lookup"><span data-stu-id="3c551-128">5</span></span>|<span data-ttu-id="3c551-129">Das Gerät wird für die Verwaltung mobiler Geräte nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c551-129">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="3c551-130">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="3c551-130">inMaintenance</span></span>|<span data-ttu-id="3c551-131">6</span><span class="sxs-lookup"><span data-stu-id="3c551-131">6</span></span>|<span data-ttu-id="3c551-132">Das Konto ist in Wartung.</span><span class="sxs-lookup"><span data-stu-id="3c551-132">Account is in maintenance.</span></span>|
|<span data-ttu-id="3c551-133">badRequest</span><span class="sxs-lookup"><span data-stu-id="3c551-133">badRequest</span></span>|<span data-ttu-id="3c551-134">7</span><span class="sxs-lookup"><span data-stu-id="3c551-134">7</span></span>|<span data-ttu-id="3c551-135">Der Client hat eine Anforderung gesendet, die vom Dienst nicht verstanden/unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="3c551-135">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="3c551-136">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="3c551-136">featureNotSupported</span></span>|<span data-ttu-id="3c551-137">8</span><span class="sxs-lookup"><span data-stu-id="3c551-137">8</span></span>|<span data-ttu-id="3c551-138">Von dieser Registrierung verwendete Features werden für dieses Konto nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3c551-138">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="3c551-139">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="3c551-139">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="3c551-140">9</span><span class="sxs-lookup"><span data-stu-id="3c551-140">9</span></span>|<span data-ttu-id="3c551-141">Durch den Administrator konfigurierte Registrierungs Einschränkungen haben diese Registrierung blockiert.</span><span class="sxs-lookup"><span data-stu-id="3c551-141">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="3c551-142">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="3c551-142">clientDisconnected</span></span>|<span data-ttu-id="3c551-143">10</span><span class="sxs-lookup"><span data-stu-id="3c551-143">10</span></span>|<span data-ttu-id="3c551-144">Timeout des Clients, oder die Registrierung wurde vom Endverbraucher abgebrochen.</span><span class="sxs-lookup"><span data-stu-id="3c551-144">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="3c551-145">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="3c551-145">userAbandonment</span></span>|<span data-ttu-id="3c551-146">11</span><span class="sxs-lookup"><span data-stu-id="3c551-146">11</span></span>|<span data-ttu-id="3c551-147">Die Registrierung wurde vom Endverbraucher abgebrochen.</span><span class="sxs-lookup"><span data-stu-id="3c551-147">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="3c551-148">(Der Endanwender hat das Onboarding gestartet, konnte es jedoch nicht rechtzeitig abschließen)</span><span class="sxs-lookup"><span data-stu-id="3c551-148">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->

