---
title: So schützen Sie Daten in Unternehmens-Apps mit Microsoft Intune
description: Die App-Schutz-Richtlinien von Microsoft Intune schützen die Daten Ihres Unternehmens und verhindern Datenverlust.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 03b0db7a2bc2b79edf0156939b9ddb8e89f84dbd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810045"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a>So schützen Sie Daten in Unternehmens-Apps mit Microsoft Intune

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.

Die App-Schutz-Richtlinien von Microsoft Intune schützen die Daten Ihres Unternehmens und verhindern Datenverlust.

Mithilfe der App-Schutz-Richtlinien von Intune können Sie die Daten Ihres Unternehmens schützen. Da die App-Schutz-Richtlinien von Intune unabhängig von Lösungen für die Verwaltung von Mobilgeräten (MDM, Mobile Device Management) eingesetzt werden können, sind die Daten Ihres Unternehmens immer geschützt, ganz gleich, ob das Gerät, auf dem sie gespeichert sind, in einer Geräteverwaltungslösung registriert ist oder nicht. Durch die Implementierung von Richtlinien auf App-Ebene können Sie den Zugriff auf Unternehmensressourcen einschränken und dafür sorgen, dass Ihre Daten jederzeit unter der vollen Kontrolle Ihrer IT-Abteilung bleiben.

Zur Verwaltung der App-Schutz-Richtlinien in Intune stehen die folgenden Graph-Ressourcen zur Verfügung:  

- [androidManagedAppProtection](intune-mam-androidmanagedappprotection.md)
- [androidManagedAppRegistration](intune-mam-androidmanagedappregistration.md)
- [androidMobileAppIdentifier](intune-mam-androidmobileappidentifier.md)
- [Art der Anwendung](intune-wip-applicationtype.md)
- [defaultManagedAppProtection](intune-mam-defaultmanagedappprotection.md)
- [iosManagedAppProtection](intune-mam-iosmanagedappprotection.md)
- [iosManagedAppRegistration](intune-mam-iosmanagedappregistration.md)
- [iosMobileAppIdentifier](intune-mam-iosmobileappidentifier.md)
- [ipRange](intune-mam-iprange.md)
- [iPv4Range](intune-mam-ipv4range.md)
- [iPv6Range](intune-mam-ipv6range.md)
- [Json](intune-mam-json.md)
- [keyValuePair](intune-mam-keyvaluepair.md)
- [App-Zwischenablage Freigabe Ebene verwaltet](intune-mam-managedappclipboardsharinglevel.md)
- [managedAppConfiguration](intune-mam-managedappconfiguration.md)
- [Verwaltete Verschlüsselungstyp für app-Daten](intune-mam-managedappdataencryptiontype.md)
- [Speicherort der verwalteten app-Daten](intune-mam-managedappdatastoragelocation.md)
- [Verwaltete app Datenübertragung Ebene](intune-mam-managedappdatatransferlevel.md)
- [managedAppDiagnosticStatus](intune-mam-managedappdiagnosticstatus.md)
- [Verwaltete app gekennzeichnet Grund](intune-mam-managedappflaggedreason.md)
- [managedAppOperation](intune-mam-managedappoperation.md)
- [Verwaltete app PIN-Zeichensatz](intune-mam-managedapppincharacterset.md)
- [managedAppPolicy](intune-mam-managedapppolicy.md)
- [managedAppPolicyDeploymentSummary](intune-mam-managedapppolicydeploymentsummary.md)
- [managedAppPolicyDeploymentSummaryPerApp](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [managedAppProtection](intune-mam-managedappprotection.md)
- [managedAppRegistration](intune-mam-managedappregistration.md)
- [managedAppStatus](intune-mam-managedappstatus.md)
- [managedAppStatusRaw](intune-mam-managedappstatusraw.md)
- [managedMobileApp](intune-mam-managedmobileapp.md)
- [mdmWindowsInformationProtectionPolicy](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [mobileAppIdentifier](intune-mam-mobileappidentifier.md)
- [proxiedDomain](intune-mam-proxieddomain.md)
- [targetedManagedAppConfiguration](intune-mam-targetedmanagedappconfiguration.md)
- [targetedManagedAppPolicyAssignment](intune-mam-targetedmanagedapppolicyassignment.md)
- [targetedManagedAppProtection](intune-mam-targetedmanagedappprotection.md)
- [windowsInformationProtection](intune-mam-windowsinformationprotection.md)
- [windowsInformationProtectionApp](intune-mam-windowsinformationprotectionapp.md)
- [windowsInformationProtectionAppLearningSummary](intune-wip-windowsinformationprotectionapplearningsummary.md)
- [windowsInformationProtectionAppLockerFile](intune-mam-windowsinformationprotectionapplockerfile.md)
- [windowsInformationProtectionDataRecoveryCertificate](intune-mam-windowsinformationprotectiondatarecoverycertificate.md)
- [windowsInformationProtectionDesktopApp](intune-mam-windowsinformationprotectiondesktopapp.md)
- [Windows Informationen Erzwingung der Mail-Schutzstufe](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [windowsInformationProtectionIPRangeCollection](intune-mam-windowsinformationprotectioniprangecollection.md)
- [windowsInformationProtectionNetworkLearningSummary](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [Anforderungen an die Windows Angaben Protection PIN Zeichen](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [windowsInformationProtectionPolicy](intune-mam-windowsinformationprotectionpolicy.md)
- [windowsInformationProtectionProxiedDomainCollection](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [windowsInformationProtectionResourceCollection](intune-mam-windowsinformationprotectionresourcecollection.md)
- [windowsInformationProtectionStoreApp](intune-mam-windowsinformationprotectionstoreapp.md)
