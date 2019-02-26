---
title: Verwalten mobiler apps mit Microsoft InTune – Microsoft Graph-API
description: Listet die Microsoft Graph-API für InTune-Endpunkte (REST) im Zusammenhang mit Mobile-App-Verwaltung (MAM) für eine mandantenorganisation auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4443c78c6ae58979b0390496d8d560bb15a90669
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150400"
---
# <a name="how-to-protect-your-company-app-data-with-microsoft-intune"></a>So schützen Sie Daten in Unternehmens-Apps mit Microsoft Intune

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.

Die App-Schutz-Richtlinien von Microsoft Intune schützen die Daten Ihres Unternehmens und verhindern Datenverlust.

Mithilfe der App-Schutz-Richtlinien von Intune können Sie die Daten Ihres Unternehmens schützen. Da InTune-App-Schutzrichtlinien unabhängig von einer beliebigen MDM-Lösung (Mobile Device Management) verwendet werden können, können Sie Sie verwenden, um die Daten Ihres Unternehmens mit oder ohne Registrierung von Geräten in einer Geräteverwaltungslösung zu schützen. Durch die Implementierung von Richtlinien auf App-Ebene können Sie den Zugriff auf Unternehmensressourcen einschränken und dafür sorgen, dass Ihre Daten jederzeit unter der vollen Kontrolle Ihrer IT-Abteilung bleiben.

Zur Verwaltung der App-Schutz-Richtlinien in Intune stehen die folgenden Graph-Ressourcen zur Verfügung:

- [androidManagedAppProtection](intune-mam-androidmanagedappprotection.md)
- [androidManagedAppRegistration](intune-mam-androidmanagedappregistration.md)
- [androidMobileAppIdentifier](intune-mam-androidmobileappidentifier.md)
- [App-Verwaltungsebene](intune-mam-appmanagementlevel.md)
- [Anwendungstyp](intune-wip-applicationtype.md)
- [defaultManagedAppProtection](intune-mam-defaultmanagedappprotection.md)
- [Intune-Brandingprofil](intune-wip-intunebrandingprofile.md)
- [Intune-Brandingprofil – Zuweisung](intune-wip-intunebrandingprofileassignment.md)
- [iosManagedAppProtection](intune-mam-iosmanagedappprotection.md)
- [iosManagedAppRegistration](intune-mam-iosmanagedappregistration.md)
- [iosMobileAppIdentifier](intune-mam-iosmobileappidentifier.md)
- [Json](intune-mam-json.md)
- [Freigabeebene der Zwischenablage verwalteter Apps](intune-mam-managedappclipboardsharinglevel.md)
- [managedAppConfiguration](intune-mam-managedappconfiguration.md)
- [Datenverschlüsselungstyp für verwaltete Apps](intune-mam-managedappdataencryptiontype.md)
- [Datenspeicherstandort für verwaltete Apps](intune-mam-managedappdatastoragelocation.md)
- [Datenübertragungsebene  für verwaltete Apps](intune-mam-managedappdatatransferlevel.md)
- [managedAppDiagnosticStatus](intune-mam-managedappdiagnosticstatus.md)
- [Grund für Kennzeichnung verwalteter App](intune-mam-managedappflaggedreason.md)
- [managedAppOperation](intune-mam-managedappoperation.md)
- [Zeichensatz für PIN verwalteter Apps](intune-mam-managedapppincharacterset.md)
- [managedAppPolicy](intune-mam-managedapppolicy.md)
- [managedAppPolicyDeploymentSummary](intune-mam-managedapppolicydeploymentsummary.md)
- [managedAppPolicyDeploymentSummaryPerApp](intune-mam-managedapppolicydeploymentsummaryperapp.md)
- [managedAppProtection](intune-mam-managedappprotection.md)
- [managedAppRegistration](intune-mam-managedappregistration.md)
- [Wartungsaktion für verwaltete Apps](intune-mam-managedappremediationaction.md)
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
- [Windows Information Protection – Geräteregistrierung](intune-mam-windowsinformationprotectiondeviceregistration.md)
- [Windows Information Protection – Erzwingungsstufe](intune-mam-windowsinformationprotectionenforcementlevel.md)
- [windowsInformationProtectionIPRangeCollection](intune-mam-windowsinformationprotectioniprangecollection.md)
- [windowsInformationProtectionNetworkLearningSummary](intune-wip-windowsinformationprotectionnetworklearningsummary.md)
- [Windows Information Protection – Anforderungen für PIN-Zeichensatz](intune-mam-windowsinformationprotectionpincharacterrequirements.md)
- [windowsInformationProtectionPolicy](intune-mam-windowsinformationprotectionpolicy.md)
- [windowsInformationProtectionProxiedDomainCollection](intune-mam-windowsinformationprotectionproxieddomaincollection.md)
- [windowsInformationProtectionResourceCollection](intune-mam-windowsinformationprotectionresourcecollection.md)
- [windowsInformationProtectionStoreApp](intune-mam-windowsinformationprotectionstoreapp.md)
- [Windows Information Protection – Zurücksetzung](intune-mam-windowsinformationprotectionwipeaction.md)
