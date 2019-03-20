---
title: Registrieren von Unternehmensgeräten mithilfe von InTune – Microsoft Graph-API
description: Listet die Microsoft Graph-API für InTune-Endpunkte (REST) auf, die Geräte für eine mandantenorganisation registrieren.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4b4100265797fd3cefc60e0288961b74839199c2
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572390"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="8c56d-103">Unternehmenseigene Geräte mit Intune registrieren</span><span class="sxs-lookup"><span data-stu-id="8c56d-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="8c56d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8c56d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c56d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c56d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c56d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="8c56d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="8c56d-107">Sie können organisations- oder unternehmenseigene Geräte für die Verwaltung in Intune auf unterschiedliche Weise und abhängig von der Art des Geräts, der Art der Anschaffung des Geräts und den Anforderungen der Organisation registrieren.</span><span class="sxs-lookup"><span data-stu-id="8c56d-107">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="8c56d-108">Sie können auch die Unternehmensportal-App installieren, um unternehmenseigene Geräte zu registrieren und verwalten, wie z. B. in einem Szenario mit geschäftlich genutzten Privatgeräten der Benutzer (BYOD).</span><span class="sxs-lookup"><span data-stu-id="8c56d-108">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="8c56d-109">Zur Verwaltung der unternehmenseigenen Geräte in Intune stehen die folgenden Graph-Ressourcen zur Verfügung:</span><span class="sxs-lookup"><span data-stu-id="8c56d-109">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="8c56d-110">Profil für Active Directory Windows Autopilot Deployment</span><span class="sxs-lookup"><span data-stu-id="8c56d-110">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="8c56d-111">Profil für Azure AD Windows Autopilot Deployment</span><span class="sxs-lookup"><span data-stu-id="8c56d-111">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="8c56d-112">DEP-Registrierung – Basisprofil</span><span class="sxs-lookup"><span data-stu-id="8c56d-112">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="8c56d-113">DEP-Registrierungsprofil</span><span class="sxs-lookup"><span data-stu-id="8c56d-113">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="8c56d-114">DEP iOS-Registrierungsprofil</span><span class="sxs-lookup"><span data-stu-id="8c56d-114">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="8c56d-115">DEP macOS-Registrierungsprofil</span><span class="sxs-lookup"><span data-stu-id="8c56d-115">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="8c56d-116">DEP-Onboarding-Einstellung</span><span class="sxs-lookup"><span data-stu-id="8c56d-116">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="8c56d-117">DEP-Tokentyp</span><span class="sxs-lookup"><span data-stu-id="8c56d-117">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="8c56d-118">Ermittlungsquelle</span><span class="sxs-lookup"><span data-stu-id="8c56d-118">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="8c56d-119">Registrierungsprofil</span><span class="sxs-lookup"><span data-stu-id="8c56d-119">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="8c56d-120">Registrierungsstatus</span><span class="sxs-lookup"><span data-stu-id="8c56d-120">Enrollment state</span></span>](intune-enrollment-enrollmentstate.md)
- [<span data-ttu-id="8c56d-121">Importierte Apple-Geräteidentität</span><span class="sxs-lookup"><span data-stu-id="8c56d-121">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="8c56d-122">Ergebnis der importierten Apple-Geräteidentität</span><span class="sxs-lookup"><span data-stu-id="8c56d-122">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="8c56d-123">Importierte Geräteidentität</span><span class="sxs-lookup"><span data-stu-id="8c56d-123">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="8c56d-124">Ergebnis der importierten Geräteidentität</span><span class="sxs-lookup"><span data-stu-id="8c56d-124">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="8c56d-125">Typ der importierten Geräteidentität</span><span class="sxs-lookup"><span data-stu-id="8c56d-125">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="8c56d-126">Importierte Windows Autopilot-Geräteidentität</span><span class="sxs-lookup"><span data-stu-id="8c56d-126">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="8c56d-127">Importstatus der importierten Windows Autopilot-Geräteidentität</span><span class="sxs-lookup"><span data-stu-id="8c56d-127">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="8c56d-128">Status der importierten Windows Autopilot-Geräteidentität</span><span class="sxs-lookup"><span data-stu-id="8c56d-128">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="8c56d-129">Upload der importierten Windows Autopilot-Geräteidentität</span><span class="sxs-lookup"><span data-stu-id="8c56d-129">Imported windows autopilot device identity upload</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [<span data-ttu-id="8c56d-130">Uploadstatus der importierten Windows Autopilot-Geräteidentität</span><span class="sxs-lookup"><span data-stu-id="8c56d-130">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="8c56d-131">iTunes-Kopplungsmodus</span><span class="sxs-lookup"><span data-stu-id="8c56d-131">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="8c56d-132">Verwaltungszertifikat mit Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="8c56d-132">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="8c56d-133">Einstellungen für Windows-Willkommensseite</span><span class="sxs-lookup"><span data-stu-id="8c56d-133">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="8c56d-134">Plattform</span><span class="sxs-lookup"><span data-stu-id="8c56d-134">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="8c56d-135">Profil für Windows Autopilot Deployment</span><span class="sxs-lookup"><span data-stu-id="8c56d-135">Windows autopilot deployment profile</span></span>](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="8c56d-136">Profilzuweisung für Windows Autopilot Deployment</span><span class="sxs-lookup"><span data-stu-id="8c56d-136">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="8c56d-137">Windows Autopilot-Geräteidentität</span><span class="sxs-lookup"><span data-stu-id="8c56d-137">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="8c56d-138">Windows Autopilot-Gerätetyp</span><span class="sxs-lookup"><span data-stu-id="8c56d-138">Windows autopilot device type</span></span>](intune-enrollment-windowsautopilotdevicetype.md)
- [<span data-ttu-id="8c56d-139">Profil für Windows Autopilot – Detaillierter Zuweisungsstatus</span><span class="sxs-lookup"><span data-stu-id="8c56d-139">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="8c56d-140">Profil für Windows Autopilot – Zuweisungsstatus</span><span class="sxs-lookup"><span data-stu-id="8c56d-140">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="8c56d-141">Windows Autopilot-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="8c56d-141">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="8c56d-142">Windows Autopilot-Synchronisierungsstatus</span><span class="sxs-lookup"><span data-stu-id="8c56d-142">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="8c56d-143">Windows-Gerätenutzungstyp</span><span class="sxs-lookup"><span data-stu-id="8c56d-143">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="8c56d-144">Bildschirmeinstellungen für Windows-Registrierungsstatus</span><span class="sxs-lookup"><span data-stu-id="8c56d-144">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="8c56d-145">Windows-Benutzertyp</span><span class="sxs-lookup"><span data-stu-id="8c56d-145">Windows user type</span></span>](intune-enrollment-windowsusertype.md)
