---
title: So schützen Sie Daten in Unternehmens-Apps mit Microsoft Intune
description: Die App-Schutz-Richtlinien von Microsoft Intune schützen die Daten Ihres Unternehmens und verhindern Datenverlust.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 323c19d689ee6f0b41e6a71270a434a9e891eb0b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835406"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a>So schützen Sie Daten in Unternehmens-Apps mit Microsoft Intune

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.

Die App-Schutz-Richtlinien von Microsoft Intune schützen die Daten Ihres Unternehmens und verhindern Datenverlust.

Mithilfe der App-Schutz-Richtlinien von Intune können Sie die Daten Ihres Unternehmens schützen. Da Richtlinien für die Intune app Schutz unabhängig von jeder datensatzverwaltungslösung Mobile-Gerät (MDM) verwendet werden können, können Sie es zum Schutz Ihres Unternehmens Daten mit oder ohne eingeschrieben Geräte in einem Gerät Management-Lösung verwenden. Durch die Implementierung von Richtlinien auf App-Ebene können Sie den Zugriff auf Unternehmensressourcen einschränken und dafür sorgen, dass Ihre Daten jederzeit unter der vollen Kontrolle Ihrer IT-Abteilung bleiben.

Zur Verwaltung der App-Schutz-Richtlinien in Intune stehen die folgenden Graph-Ressourcen zur Verfügung:

- [androidManagedAppProtection](intune-mam-androidmanagedappprotection.md)
- [androidManagedAppRegistration](intune-mam-androidmanagedappregistration.md)
- [androidMobileAppIdentifier](intune-mam-androidmobileappidentifier.md)
- [App Management-Ebene](intune-mam-appmanagementlevel.md)
- [Art der Anwendung](intune-wip-applicationtype.md)
- [defaultManagedAppProtection](intune-mam-defaultmanagedappprotection.md)
- [Intune branding-Profil](intune-wip-intunebrandingprofile.md)
- [iosManagedAppProtection](intune-mam-iosmanagedappprotection.md)
- [iosManagedAppRegistration](intune-mam-iosmanagedappregistration.md)
- [iosMobileAppIdentifier](intune-mam-iosmobileappidentifier.md)
- [Json](intune-mam-json.md)
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
- [Verwaltete app Remediation-Aktion](intune-mam-managedappremediationaction.md)
- [managedAppStatus](intune-mam-managedappstatus.md)
- [managedAppStatusRaw](intune-mam-managedappstatusraw.md)
- [managedMobileApp](intune-mam-managedmobileapp.md)
- [mdmWindowsInformationProtectionPolicy](intune-mam-mdmwindowsinformationprotectionpolicy.md)
- [mobileAppIdentifier](intune-mam-mobileappidentifier.md)
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
