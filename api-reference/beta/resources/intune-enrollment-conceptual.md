---
title: Unternehmenseigene Geräte mit Intune registrieren
description: " Szenario (BYOD)."
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9671eb7f66be78075209906a4f6f923256afef36
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928024"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="2e90b-103">Unternehmenseigene Geräte mit Intune registrieren</span><span class="sxs-lookup"><span data-stu-id="2e90b-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="2e90b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2e90b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e90b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2e90b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e90b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="2e90b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="2e90b-107">Sie können organisations- oder unternehmenseigene Geräte für die Verwaltung in Intune auf unterschiedliche Weise und abhängig von der Art des Geräts, der Art der Anschaffung des Geräts und den Anforderungen der Organisation registrieren.</span><span class="sxs-lookup"><span data-stu-id="2e90b-107">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="2e90b-108">Sie können auch die Unternehmensportal-App installieren, um unternehmenseigene Geräte zu registrieren und verwalten, wie z. B. in einem Szenario mit geschäftlich genutzten Privatgeräten der Benutzer (BYOD).</span><span class="sxs-lookup"><span data-stu-id="2e90b-108">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="2e90b-109">Zur Verwaltung der unternehmenseigenen Geräte in Intune stehen die folgenden Graph-Ressourcen zur Verfügung:</span><span class="sxs-lookup"><span data-stu-id="2e90b-109">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="2e90b-110">Active Directory Windows Autopilot Bereitstellung Benutzerprofil</span><span class="sxs-lookup"><span data-stu-id="2e90b-110">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="2e90b-111">Azure AD Windows Autopilot Bereitstellung Benutzerprofil</span><span class="sxs-lookup"><span data-stu-id="2e90b-111">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="2e90b-112">Datenausführungsverhinderung Registrierung Profil</span><span class="sxs-lookup"><span data-stu-id="2e90b-112">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="2e90b-113">Datenausführungsverhinderung Registrierung Profil</span><span class="sxs-lookup"><span data-stu-id="2e90b-113">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="2e90b-114">Datenausführungsverhinderung iOS Registrierung Profil</span><span class="sxs-lookup"><span data-stu-id="2e90b-114">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="2e90b-115">Datenausführungsverhinderung Mac OS Registrierung Profil</span><span class="sxs-lookup"><span data-stu-id="2e90b-115">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="2e90b-116">DEP auf mittels Fingereingabe-Einstellung</span><span class="sxs-lookup"><span data-stu-id="2e90b-116">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="2e90b-117">Datenausführungsverhinderung token-Typ</span><span class="sxs-lookup"><span data-stu-id="2e90b-117">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="2e90b-118">Discovery-Quelle</span><span class="sxs-lookup"><span data-stu-id="2e90b-118">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="2e90b-119">Registrierung Profil</span><span class="sxs-lookup"><span data-stu-id="2e90b-119">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="2e90b-120">Status der Registrierung</span><span class="sxs-lookup"><span data-stu-id="2e90b-120">Enrollment state</span></span>](intune-enrollment-enrollmentstate.md)
- [<span data-ttu-id="2e90b-121">Importierte Apple Gerät Identität</span><span class="sxs-lookup"><span data-stu-id="2e90b-121">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="2e90b-122">Apple Gerät Identität Ergebnis importiert</span><span class="sxs-lookup"><span data-stu-id="2e90b-122">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="2e90b-123">Importierte Gerät Identität</span><span class="sxs-lookup"><span data-stu-id="2e90b-123">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="2e90b-124">Importiert Gerät Identität Ergebnis</span><span class="sxs-lookup"><span data-stu-id="2e90b-124">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="2e90b-125">Gerätetyp Identität importiert</span><span class="sxs-lookup"><span data-stu-id="2e90b-125">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="2e90b-126">Importierte Windows Autopilot Gerät Identität</span><span class="sxs-lookup"><span data-stu-id="2e90b-126">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="2e90b-127">Importierte Windows Autopilot Identität Import Gerätestatus</span><span class="sxs-lookup"><span data-stu-id="2e90b-127">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="2e90b-128">Importierte Windows Identity Autopilot Gerätestatus</span><span class="sxs-lookup"><span data-stu-id="2e90b-128">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="2e90b-129">Importierte Windows Autopilot Gerät Identität hochladen</span><span class="sxs-lookup"><span data-stu-id="2e90b-129">Imported windows autopilot device identity upload</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [<span data-ttu-id="2e90b-130">Importierte Windows Autopilot Identität Upload Gerätestatus</span><span class="sxs-lookup"><span data-stu-id="2e90b-130">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="2e90b-131">iTunes paarungs-Modus</span><span class="sxs-lookup"><span data-stu-id="2e90b-131">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="2e90b-132">Management-Zertifikat mit dem Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="2e90b-132">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="2e90b-133">Erleben Sie die Einstellungen im Lieferzustand</span><span class="sxs-lookup"><span data-stu-id="2e90b-133">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="2e90b-134">Plattform</span><span class="sxs-lookup"><span data-stu-id="2e90b-134">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="2e90b-135">Windows Autopilot Bereitstellung Benutzerprofil</span><span class="sxs-lookup"><span data-stu-id="2e90b-135">Windows autopilot deployment profile</span></span>](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="2e90b-136">Windows Autopilot Bereitstellung Profil Zuordnung</span><span class="sxs-lookup"><span data-stu-id="2e90b-136">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="2e90b-137">Windows Autopilot Gerät Identität</span><span class="sxs-lookup"><span data-stu-id="2e90b-137">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="2e90b-138">Windows Autopilot Profil Zuordnung detaillierter status</span><span class="sxs-lookup"><span data-stu-id="2e90b-138">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="2e90b-139">Zuordnung des Status von Windows Autopilot Profil</span><span class="sxs-lookup"><span data-stu-id="2e90b-139">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="2e90b-140">Windows Autopilot-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="2e90b-140">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="2e90b-141">Windows Autopilot Synchronisierungsstatus</span><span class="sxs-lookup"><span data-stu-id="2e90b-141">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="2e90b-142">Windows-Gerät Verwendungstyp</span><span class="sxs-lookup"><span data-stu-id="2e90b-142">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="2e90b-143">Windows-Registrierung Status Bildschirm-Einstellungen</span><span class="sxs-lookup"><span data-stu-id="2e90b-143">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="2e90b-144">Windows-Benutzertyp</span><span class="sxs-lookup"><span data-stu-id="2e90b-144">Windows user type</span></span>](intune-enrollment-windowsusertype.md)
