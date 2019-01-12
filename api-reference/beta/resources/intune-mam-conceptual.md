---
title: So schützen Sie Daten in Unternehmens-Apps mit Microsoft Intune
description: Die App-Schutz-Richtlinien von Microsoft Intune schützen die Daten Ihres Unternehmens und verhindern Datenverlust.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ca628b81015527cb5ab7e508bebbb2808cdcde7e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925455"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a><span data-ttu-id="cdf51-103">So schützen Sie Daten in Unternehmens-Apps mit Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="cdf51-103">How to protect your company app data with Microsoft Intune</span></span>

> <span data-ttu-id="cdf51-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cdf51-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cdf51-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cdf51-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cdf51-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="cdf51-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="cdf51-107">Die App-Schutz-Richtlinien von Microsoft Intune schützen die Daten Ihres Unternehmens und verhindern Datenverlust.</span><span class="sxs-lookup"><span data-stu-id="cdf51-107">Microsoft Intune app protection policies help protect your company data and prevent data loss.</span></span>

<span data-ttu-id="cdf51-108">Mithilfe der App-Schutz-Richtlinien von Intune können Sie die Daten Ihres Unternehmens schützen.</span><span class="sxs-lookup"><span data-stu-id="cdf51-108">You can use Intune app protection policies to help protect your company’s data.</span></span> <span data-ttu-id="cdf51-109">Da Richtlinien für die Intune app Schutz unabhängig von jeder datensatzverwaltungslösung Mobile-Gerät (MDM) verwendet werden können, können Sie es zum Schutz Ihres Unternehmens Daten mit oder ohne eingeschrieben Geräte in einem Gerät Management-Lösung verwenden.</span><span class="sxs-lookup"><span data-stu-id="cdf51-109">Because Intune app protection policies can be used independent of any mobile-device management (MDM) solution, you can use it to protect your company’s data with or without enrolling devices in a device management solution.</span></span> <span data-ttu-id="cdf51-110">Durch die Implementierung von Richtlinien auf App-Ebene können Sie den Zugriff auf Unternehmensressourcen einschränken und dafür sorgen, dass Ihre Daten jederzeit unter der vollen Kontrolle Ihrer IT-Abteilung bleiben.</span><span class="sxs-lookup"><span data-stu-id="cdf51-110">By implementing app-level policies, you can restrict access to company resources and keep data within the purview of your IT department.</span></span>

<span data-ttu-id="cdf51-111">Zur Verwaltung der App-Schutz-Richtlinien in Intune stehen die folgenden Graph-Ressourcen zur Verfügung:</span><span class="sxs-lookup"><span data-stu-id="cdf51-111">The following Graph resources are available to manage app protection polices in Intune:</span></span>

- [<span data-ttu-id="cdf51-112">androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="cdf51-112">Android managed app protection</span></span>](intune-mam-androidmanagedappprotection.md)
- [<span data-ttu-id="cdf51-113">androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="cdf51-113">Android managed app registration</span></span>](intune-mam-androidmanagedappregistration.md)
- [<span data-ttu-id="cdf51-114">androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="cdf51-114">Android mobile app identifier</span></span>](intune-mam-androidmobileappidentifier.md)
- [<span data-ttu-id="cdf51-115">App Management-Ebene</span><span class="sxs-lookup"><span data-stu-id="cdf51-115">App management level</span></span>](intune-mam-appmanagementlevel.md)
- [<span data-ttu-id="cdf51-116">Art der Anwendung</span><span class="sxs-lookup"><span data-stu-id="cdf51-116">Application type</span></span>](intune-wip-applicationtype.md)
- [<span data-ttu-id="cdf51-117">defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="cdf51-117">Default managed app protection</span></span>](intune-mam-defaultmanagedappprotection.md)
- [<span data-ttu-id="cdf51-118">Intune branding-Profil</span><span class="sxs-lookup"><span data-stu-id="cdf51-118">Intune branding profile</span></span>](intune-wip-intunebrandingprofile.md)
- [<span data-ttu-id="cdf51-119">iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="cdf51-119">iOS managed app protection</span></span>](intune-mam-iosmanagedappprotection.md)
- [<span data-ttu-id="cdf51-120">iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="cdf51-120">iOS managed app registration</span></span>](intune-mam-iosmanagedappregistration.md)
- [<span data-ttu-id="cdf51-121">iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="cdf51-121">iOS mobile app identifier</span></span>](intune-mam-iosmobileappidentifier.md)
- [<span data-ttu-id="cdf51-122">Json</span><span class="sxs-lookup"><span data-stu-id="cdf51-122">JSON</span></span>](intune-mam-json.md)
- [<span data-ttu-id="cdf51-123">App-Zwischenablage Freigabe Ebene verwaltet</span><span class="sxs-lookup"><span data-stu-id="cdf51-123">Managed app clipboard sharing level</span></span>](intune-mam-managedappclipboardsharinglevel.md)
- [<span data-ttu-id="cdf51-124">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cdf51-124">Managed app configuration</span></span>](intune-mam-managedappconfiguration.md)
- [<span data-ttu-id="cdf51-125">Verwaltete Verschlüsselungstyp für app-Daten</span><span class="sxs-lookup"><span data-stu-id="cdf51-125">Managed app data encryption type</span></span>](intune-mam-managedappdataencryptiontype.md)
- [<span data-ttu-id="cdf51-126">Speicherort der verwalteten app-Daten</span><span class="sxs-lookup"><span data-stu-id="cdf51-126">Managed app data storage location</span></span>](intune-mam-managedappdatastoragelocation.md)
- [<span data-ttu-id="cdf51-127">Verwaltete app Datenübertragung Ebene</span><span class="sxs-lookup"><span data-stu-id="cdf51-127">Managed app data transfer level</span></span>](intune-mam-managedappdatatransferlevel.md)
- [<span data-ttu-id="cdf51-128">managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="cdf51-128">Managed app diagnostic status</span></span>](intune-mam-managedappdiagnosticstatus.md)
- [<span data-ttu-id="cdf51-129">Verwaltete app gekennzeichnet Grund</span><span class="sxs-lookup"><span data-stu-id="cdf51-129">Managed app flagged reason</span></span>](intune-mam-managedappflaggedreason.md)
- [<span data-ttu-id="cdf51-130">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="cdf51-130">Managed app operation</span></span>](intune-mam-managedappoperation.md)
- [<span data-ttu-id="cdf51-131">Verwaltete app PIN-Zeichensatz</span><span class="sxs-lookup"><span data-stu-id="cdf51-131">Managed app PIN character set</span></span>](intune-mam-managedapppincharacterset.md)
- [<span data-ttu-id="cdf51-132">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="cdf51-132">Managed app policy</span></span>](intune-mam-managedapppolicy.md)
- [<span data-ttu-id="cdf51-133">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="cdf51-133">Managed app policy deployment summary</span></span>](intune-mam-managedapppolicydeploymentsummary.md)
- [<span data-ttu-id="cdf51-134">managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="cdf51-134">Managed app policy deployment summary per app</span></span>](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [<span data-ttu-id="cdf51-135">managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="cdf51-135">Managed app protection</span></span>](intune-mam-managedappprotection.md)
- [<span data-ttu-id="cdf51-136">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="cdf51-136">Managed app registration</span></span>](intune-mam-managedappregistration.md)
- [<span data-ttu-id="cdf51-137">Verwaltete app Remediation-Aktion</span><span class="sxs-lookup"><span data-stu-id="cdf51-137">Managed app remediation action</span></span>](intune-mam-managedappremediationaction.md)
- [<span data-ttu-id="cdf51-138">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="cdf51-138">Managed app status</span></span>](intune-mam-managedappstatus.md)
- [<span data-ttu-id="cdf51-139">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="cdf51-139">Managed app status raw</span></span>](intune-mam-managedappstatusraw.md)
- [<span data-ttu-id="cdf51-140">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="cdf51-140">Managed mobile app</span></span>](intune-mam-managedmobileapp.md)
- [<span data-ttu-id="cdf51-141">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="cdf51-141">MDM windows information protection policy</span></span>](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="cdf51-142">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="cdf51-142">Mobile app identifier</span></span>](intune-mam-mobileappidentifier.md)
- [<span data-ttu-id="cdf51-143">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cdf51-143">Targeted managed app configuration</span></span>](intune-mam-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="cdf51-144">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="cdf51-144">Targeted managed app policy assignment</span></span>](intune-mam-targetedmanagedapppolicyassignment.md)
- [<span data-ttu-id="cdf51-145">targetedManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="cdf51-145">Targeted managed app protection</span></span>](intune-mam-targetedmanagedappprotection.md)
- [<span data-ttu-id="cdf51-146">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="cdf51-146">Windows information protection</span></span>](intune-mam-windowsinformationprotection.md)
- [<span data-ttu-id="cdf51-147">windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="cdf51-147">Windows information protection app</span></span>](intune-mam-windowsinformationprotectionapp.md)
- [<span data-ttu-id="cdf51-148">windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="cdf51-148">Windows information protection app learning summary</span></span>](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [<span data-ttu-id="cdf51-149">windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="cdf51-149">Windows information protection app locker file</span></span>](intune-mam-windowsinformationprotectionapplockerfile.md)
- [<span data-ttu-id="cdf51-150">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="cdf51-150">Windows information protection data recovery certificate</span></span>](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [<span data-ttu-id="cdf51-151">windowsInformationProtectionDesktopApp</span><span class="sxs-lookup"><span data-stu-id="cdf51-151">Windows information protection desktop app</span></span>](intune-mam-windowsinformationprotectiondesktopapp.md)
- [<span data-ttu-id="cdf51-152">Windows Informationen Erzwingung der Mail-Schutzstufe</span><span class="sxs-lookup"><span data-stu-id="cdf51-152">Windows information protection enforcement level</span></span>](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [<span data-ttu-id="cdf51-153">windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="cdf51-153">Windows information protection IP range collection</span></span>](intune-mam-windowsinformationprotectioniprangecollection.md)
- [<span data-ttu-id="cdf51-154">windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="cdf51-154">Windows information protection network learning summary</span></span>](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [<span data-ttu-id="cdf51-155">Anforderungen an die Windows Angaben Protection PIN Zeichen</span><span class="sxs-lookup"><span data-stu-id="cdf51-155">Windows information protection PIN character requirements</span></span>](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [<span data-ttu-id="cdf51-156">windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="cdf51-156">Windows information protection policy</span></span>](intune-mam-windowsinformationprotectionpolicy.md)
- [<span data-ttu-id="cdf51-157">windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="cdf51-157">Windows information protection proxied domain collection</span></span>](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [<span data-ttu-id="cdf51-158">windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="cdf51-158">Windows information protection resource collection</span></span>](intune-mam-windowsinformationprotectionresourcecollection.md)
- [<span data-ttu-id="cdf51-159">windowsInformationProtectionStoreApp</span><span class="sxs-lookup"><span data-stu-id="cdf51-159">Windows information protection store app</span></span>](intune-mam-windowsinformationprotectionstoreapp.md)
