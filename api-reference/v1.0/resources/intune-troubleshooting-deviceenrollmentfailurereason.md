---
title: DeviceEnrollmentFailureReason Enum-Typ
description: Oberste Ebene Fehler Kategorien für die Registrierung.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: efee4e4655d36e7575df9e0ddda508dbbcc473c5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962072"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="d2ce9-103">DeviceEnrollmentFailureReason Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="d2ce9-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="d2ce9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d2ce9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2ce9-105">Oberste Ebene Fehler Kategorien für die Registrierung.</span><span class="sxs-lookup"><span data-stu-id="d2ce9-105">Top level failure categories for enrollment.</span></span>
## <a name="members"></a><span data-ttu-id="d2ce9-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="d2ce9-106">Members</span></span>
|<span data-ttu-id="d2ce9-107">Element</span><span class="sxs-lookup"><span data-stu-id="d2ce9-107">Member</span></span>|<span data-ttu-id="d2ce9-108">Wert</span><span class="sxs-lookup"><span data-stu-id="d2ce9-108">Value</span></span>|<span data-ttu-id="d2ce9-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d2ce9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2ce9-110">unknown</span><span class="sxs-lookup"><span data-stu-id="d2ce9-110">unknown</span></span>|<span data-ttu-id="d2ce9-111">0</span><span class="sxs-lookup"><span data-stu-id="d2ce9-111">0</span></span>|<span data-ttu-id="d2ce9-112">Der Standardwert, Fehlerursache ist unbekannt.</span><span class="sxs-lookup"><span data-stu-id="d2ce9-112">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="d2ce9-113">Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="d2ce9-113">authentication</span></span>|<span data-ttu-id="d2ce9-114">1</span><span class="sxs-lookup"><span data-stu-id="d2ce9-114">1</span></span>|<span data-ttu-id="d2ce9-115">Fehler bei der Authentifizierung</span><span class="sxs-lookup"><span data-stu-id="d2ce9-115">Authentication failed</span></span>|
|<span data-ttu-id="d2ce9-116">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="d2ce9-116">authorization</span></span>|<span data-ttu-id="d2ce9-117">2</span><span class="sxs-lookup"><span data-stu-id="d2ce9-117">2</span></span>|<span data-ttu-id="d2ce9-118">Anruf wurde authentifiziert, jedoch nicht autorisiert, registrieren.</span><span class="sxs-lookup"><span data-stu-id="d2ce9-118">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="d2ce9-119">accountValidation</span><span class="sxs-lookup"><span data-stu-id="d2ce9-119">accountValidation</span></span>|<span data-ttu-id="d2ce9-120">3</span><span class="sxs-lookup"><span data-stu-id="d2ce9-120">3</span></span>|<span data-ttu-id="d2ce9-121">Fehler beim Überprüfen von des Kontos für die Registrierung.</span><span class="sxs-lookup"><span data-stu-id="d2ce9-121">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="d2ce9-122">(Konto blockiert, Registrierung nicht aktiviert)</span><span class="sxs-lookup"><span data-stu-id="d2ce9-122">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="d2ce9-123">userValidation</span><span class="sxs-lookup"><span data-stu-id="d2ce9-123">userValidation</span></span>|<span data-ttu-id="d2ce9-124">4</span><span class="sxs-lookup"><span data-stu-id="d2ce9-124">4</span></span>|<span data-ttu-id="d2ce9-125">Benutzer konnte nicht überprüft werden.</span><span class="sxs-lookup"><span data-stu-id="d2ce9-125">User could not be validated.</span></span> <span data-ttu-id="d2ce9-126">(Benutzer ist nicht vorhanden, fehlende Lizenz)</span><span class="sxs-lookup"><span data-stu-id="d2ce9-126">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="d2ce9-127">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="d2ce9-127">deviceNotSupported</span></span>|<span data-ttu-id="d2ce9-128">5</span><span class="sxs-lookup"><span data-stu-id="d2ce9-128">5</span></span>|<span data-ttu-id="d2ce9-129">Gerät ist nicht für die Verwaltung von mobilen Geräten unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d2ce9-129">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="d2ce9-130">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="d2ce9-130">inMaintenance</span></span>|<span data-ttu-id="d2ce9-131">6</span><span class="sxs-lookup"><span data-stu-id="d2ce9-131">6</span></span>|<span data-ttu-id="d2ce9-132">Konto ist in der Wartung.</span><span class="sxs-lookup"><span data-stu-id="d2ce9-132">Account is in maintenance.</span></span>|
|<span data-ttu-id="d2ce9-133">badRequest</span><span class="sxs-lookup"><span data-stu-id="d2ce9-133">badRequest</span></span>|<span data-ttu-id="d2ce9-134">7</span><span class="sxs-lookup"><span data-stu-id="d2ce9-134">7</span></span>|<span data-ttu-id="d2ce9-135">Client gesendet eine Anforderung, die nicht vom Dienst verstanden/unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="d2ce9-135">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="d2ce9-136">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="d2ce9-136">featureNotSupported</span></span>|<span data-ttu-id="d2ce9-137">8</span><span class="sxs-lookup"><span data-stu-id="d2ce9-137">8</span></span>|<span data-ttu-id="d2ce9-138">Features, die durch diese Registrierung verwendet werden für dieses Konto nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d2ce9-138">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="d2ce9-139">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="d2ce9-139">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="d2ce9-140">9</span><span class="sxs-lookup"><span data-stu-id="d2ce9-140">9</span></span>|<span data-ttu-id="d2ce9-141">Registrierung Einschränkungen durch den Administrator konfiguriert blockiert diese Registrierung.</span><span class="sxs-lookup"><span data-stu-id="d2ce9-141">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="d2ce9-142">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="d2ce9-142">clientDisconnected</span></span>|<span data-ttu-id="d2ce9-143">10</span><span class="sxs-lookup"><span data-stu-id="d2ce9-143">10</span></span>|<span data-ttu-id="d2ce9-144">Client ein Timeout aufgetreten, oder die Registrierung mithilfe des Endbenutzers abgebrochen wurde.</span><span class="sxs-lookup"><span data-stu-id="d2ce9-144">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="d2ce9-145">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="d2ce9-145">userAbandonment</span></span>|<span data-ttu-id="d2ce9-146">11</span><span class="sxs-lookup"><span data-stu-id="d2ce9-146">11</span></span>|<span data-ttu-id="d2ce9-147">Registrierung wurde abgebrochen, mithilfe des Endbenutzers.</span><span class="sxs-lookup"><span data-stu-id="d2ce9-147">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="d2ce9-148">(Des Endbenutzers Onboarding gestartet, aber nicht in kurzer Zeit abgeschlossen)</span><span class="sxs-lookup"><span data-stu-id="d2ce9-148">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->
