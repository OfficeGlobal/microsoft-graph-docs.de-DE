---
title: So schützen Sie Daten in Unternehmens-Apps mit Microsoft Intune
description: Die App-Schutz-Richtlinien von Microsoft Intune schützen die Daten Ihres Unternehmens und verhindern Datenverlust.
author: tfitzmac
ms.openlocfilehash: d50b86b8ef1afe1cc6ddec125b3679c605979c88
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340320"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a><span data-ttu-id="fd7d2-103">So schützen Sie Daten in Unternehmens-Apps mit Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="fd7d2-103">How to protect your company app data with Microsoft Intune</span></span>

> <span data-ttu-id="fd7d2-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="fd7d2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="fd7d2-105">Die App-Schutz-Richtlinien von Microsoft Intune schützen die Daten Ihres Unternehmens und verhindern Datenverlust.</span><span class="sxs-lookup"><span data-stu-id="fd7d2-105">Microsoft Intune app protection policies help protect your company data and prevent data loss.</span></span>

<span data-ttu-id="fd7d2-106">Mithilfe der App-Schutz-Richtlinien von Intune können Sie die Daten Ihres Unternehmens schützen.</span><span class="sxs-lookup"><span data-stu-id="fd7d2-106">You can use Intune app protection policies to help protect your company’s data.</span></span> <span data-ttu-id="fd7d2-107">Da die App-Schutz-Richtlinien von Intune unabhängig von Lösungen für die Verwaltung von Mobilgeräten (MDM, Mobile Device Management) eingesetzt werden können, sind die Daten Ihres Unternehmens immer geschützt, ganz gleich, ob das Gerät, auf dem sie gespeichert sind, in einer Geräteverwaltungslösung registriert ist oder nicht.</span><span class="sxs-lookup"><span data-stu-id="fd7d2-107">Because Intune app protection policies can be used independent of any mobile-device management (MDM) solution, you protect your company’s data with or without enrolling devices in a device management solution.</span></span> <span data-ttu-id="fd7d2-108">Durch die Implementierung von Richtlinien auf App-Ebene können Sie den Zugriff auf Unternehmensressourcen einschränken und dafür sorgen, dass Ihre Daten jederzeit unter der vollen Kontrolle Ihrer IT-Abteilung bleiben.</span><span class="sxs-lookup"><span data-stu-id="fd7d2-108">By implementing app-level policies, you can restrict access to company resources and keep data within the purview of your IT department.</span></span>

<span data-ttu-id="fd7d2-109">Zur Verwaltung der App-Schutz-Richtlinien in Intune stehen die folgenden Graph-Ressourcen zur Verfügung:</span><span class="sxs-lookup"><span data-stu-id="fd7d2-109">The following Graph resources are available to manage app protection polices in Intune:</span></span>  

- [<span data-ttu-id="fd7d2-110">androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="fd7d2-110">Android managed app protection</span></span>](intune-mam-androidmanagedappprotection.md)
- [<span data-ttu-id="fd7d2-111">androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="fd7d2-111">Android managed app registration</span></span>](intune-mam-androidmanagedappregistration.md)
- [<span data-ttu-id="fd7d2-112">androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fd7d2-112">Android mobile app identifier</span></span>](intune-mam-androidmobileappidentifier.md)
- [<span data-ttu-id="fd7d2-113">Art der Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd7d2-113">Application type</span></span>](intune-wip-applicationtype.md)
- [<span data-ttu-id="fd7d2-114">defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="fd7d2-114">Default managed app protection</span></span>](intune-mam-defaultmanagedappprotection.md)
- [<span data-ttu-id="fd7d2-115">iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="fd7d2-115">iOS managed app protection</span></span>](intune-mam-iosmanagedappprotection.md)
- [<span data-ttu-id="fd7d2-116">iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="fd7d2-116">iOS managed app registration</span></span>](intune-mam-iosmanagedappregistration.md)
- [<span data-ttu-id="fd7d2-117">iosMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fd7d2-117">iOS mobile app identifier</span></span>](intune-mam-iosmobileappidentifier.md)
- [<span data-ttu-id="fd7d2-118">ipRange</span><span class="sxs-lookup"><span data-stu-id="fd7d2-118">IP range</span></span>](intune-mam-iprange.md)
- [<span data-ttu-id="fd7d2-119">iPv4Range</span><span class="sxs-lookup"><span data-stu-id="fd7d2-119">IPv4 range</span></span>](intune-mam-ipv4range.md)
- [<span data-ttu-id="fd7d2-120">iPv6Range</span><span class="sxs-lookup"><span data-stu-id="fd7d2-120">IPv6 range</span></span>](intune-mam-ipv6range.md)
- [<span data-ttu-id="fd7d2-121">Json</span><span class="sxs-lookup"><span data-stu-id="fd7d2-121">JSON</span></span>](intune-mam-json.md)
- [<span data-ttu-id="fd7d2-122">keyValuePair</span><span class="sxs-lookup"><span data-stu-id="fd7d2-122">Key/value pair</span></span>](intune-mam-keyvaluepair.md)
- [<span data-ttu-id="fd7d2-123">App-Zwischenablage Freigabe Ebene verwaltet</span><span class="sxs-lookup"><span data-stu-id="fd7d2-123">Managed app clipboard sharing level</span></span>](intune-mam-managedappclipboardsharinglevel.md)
- [<span data-ttu-id="fd7d2-124">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd7d2-124">Managed app configuration</span></span>](intune-mam-managedappconfiguration.md)
- [<span data-ttu-id="fd7d2-125">Verwaltete Verschlüsselungstyp für app-Daten</span><span class="sxs-lookup"><span data-stu-id="fd7d2-125">Managed app data encryption type</span></span>](intune-mam-managedappdataencryptiontype.md)
- [<span data-ttu-id="fd7d2-126">Speicherort der verwalteten app-Daten</span><span class="sxs-lookup"><span data-stu-id="fd7d2-126">Managed app data storage location</span></span>](intune-mam-managedappdatastoragelocation.md)
- [<span data-ttu-id="fd7d2-127">Verwaltete app Datenübertragung Ebene</span><span class="sxs-lookup"><span data-stu-id="fd7d2-127">Managed app data transfer level</span></span>](intune-mam-managedappdatatransferlevel.md)
- [<span data-ttu-id="fd7d2-128">managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="fd7d2-128">Managed app diagnostic status</span></span>](intune-mam-managedappdiagnosticstatus.md)
- [<span data-ttu-id="fd7d2-129">Verwaltete app gekennzeichnet Grund</span><span class="sxs-lookup"><span data-stu-id="fd7d2-129">Managed app flagged reason</span></span>](intune-mam-managedappflaggedreason.md)
- [<span data-ttu-id="fd7d2-130">managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="fd7d2-130">Managed app operation</span></span>](intune-mam-managedappoperation.md)
- [<span data-ttu-id="fd7d2-131">Verwaltete app PIN-Zeichensatz</span><span class="sxs-lookup"><span data-stu-id="fd7d2-131">Managed app PIN character set</span></span>](intune-mam-managedapppincharacterset.md)
- [<span data-ttu-id="fd7d2-132">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="fd7d2-132">Managed app policy</span></span>](intune-mam-managedapppolicy.md)
- [<span data-ttu-id="fd7d2-133">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="fd7d2-133">Managed app policy deployment summary</span></span>](intune-mam-managedapppolicydeploymentsummary.md)
- [<span data-ttu-id="fd7d2-134">managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="fd7d2-134">Managed app policy deployment summary per app</span></span>](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [<span data-ttu-id="fd7d2-135">managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="fd7d2-135">Managed app protection</span></span>](intune-mam-managedappprotection.md)
- [<span data-ttu-id="fd7d2-136">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="fd7d2-136">Managed app registration</span></span>](intune-mam-managedappregistration.md)
- [<span data-ttu-id="fd7d2-137">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="fd7d2-137">Managed app status</span></span>](intune-mam-managedappstatus.md)
- [<span data-ttu-id="fd7d2-138">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="fd7d2-138">Managed app status raw</span></span>](intune-mam-managedappstatusraw.md)
- [<span data-ttu-id="fd7d2-139">managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="fd7d2-139">Managed mobile app</span></span>](intune-mam-managedmobileapp.md)
- [<span data-ttu-id="fd7d2-140">mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fd7d2-140">MDM windows information protection policy</span></span>](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [<span data-ttu-id="fd7d2-141">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fd7d2-141">Mobile app identifier</span></span>](intune-mam-mobileappidentifier.md)
- [<span data-ttu-id="fd7d2-142">proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="fd7d2-142">Proxied domain</span></span>](intune-mam-proxieddomain.md)
- [<span data-ttu-id="fd7d2-143">targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="fd7d2-143">Targeted managed app configuration</span></span>](intune-mam-targetedmanagedappconfiguration.md)
- [<span data-ttu-id="fd7d2-144">targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="fd7d2-144">Targeted managed app policy assignment</span></span>](intune-mam-targetedmanagedapppolicyassignment.md)
- [<span data-ttu-id="fd7d2-145">targetedManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="fd7d2-145">Targeted managed app protection</span></span>](intune-mam-targetedmanagedappprotection.md)
- [<span data-ttu-id="fd7d2-146">windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="fd7d2-146">Windows information protection</span></span>](intune-mam-windowsinformationprotection.md)
- [<span data-ttu-id="fd7d2-147">windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="fd7d2-147">Windows information protection app</span></span>](intune-mam-windowsinformationprotectionapp.md)
- [<span data-ttu-id="fd7d2-148">windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="fd7d2-148">Windows information protection app learning summary</span></span>](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [<span data-ttu-id="fd7d2-149">windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="fd7d2-149">Windows information protection app locker file</span></span>](intune-mam-windowsinformationprotectionapplockerfile.md)
- [<span data-ttu-id="fd7d2-150">windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="fd7d2-150">Windows information protection data recovery certificate</span></span>](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [<span data-ttu-id="fd7d2-151">windowsInformationProtectionDesktopApp</span><span class="sxs-lookup"><span data-stu-id="fd7d2-151">Windows information protection desktop app</span></span>](intune-mam-windowsinformationprotectiondesktopapp.md)
- [<span data-ttu-id="fd7d2-152">Windows Informationen Erzwingung der Mail-Schutzstufe</span><span class="sxs-lookup"><span data-stu-id="fd7d2-152">Windows information protection enforcement level</span></span>](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [<span data-ttu-id="fd7d2-153">windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="fd7d2-153">Windows information protection IP range collection</span></span>](intune-mam-windowsinformationprotectioniprangecollection.md)
- [<span data-ttu-id="fd7d2-154">windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="fd7d2-154">Windows information protection network learning summary</span></span>](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [<span data-ttu-id="fd7d2-155">Anforderungen an die Windows Angaben Protection PIN Zeichen</span><span class="sxs-lookup"><span data-stu-id="fd7d2-155">Windows information protection PIN character requirements</span></span>](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [<span data-ttu-id="fd7d2-156">windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fd7d2-156">Windows information protection policy</span></span>](intune-mam-windowsinformationprotectionpolicy.md)
- [<span data-ttu-id="fd7d2-157">windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="fd7d2-157">Windows information protection proxied domain collection</span></span>](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [<span data-ttu-id="fd7d2-158">windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="fd7d2-158">Windows information protection resource collection</span></span>](intune-mam-windowsinformationprotectionresourcecollection.md)
- [<span data-ttu-id="fd7d2-159">windowsInformationProtectionStoreApp</span><span class="sxs-lookup"><span data-stu-id="fd7d2-159">Windows information protection store app</span></span>](intune-mam-windowsinformationprotectionstoreapp.md)
