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
# <a name="enroll-corporate-owned-devices-by-using-intune"></a>Unternehmenseigene Geräte mit Intune registrieren

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.

Sie können organisations- oder unternehmenseigene Geräte für die Verwaltung in Intune auf unterschiedliche Weise und abhängig von der Art des Geräts, der Art der Anschaffung des Geräts und den Anforderungen der Organisation registrieren. Sie können auch die Unternehmensportal-App installieren, um unternehmenseigene Geräte zu registrieren und verwalten, wie z. B. in einem Szenario mit geschäftlich genutzten Privatgeräten der Benutzer (BYOD).

Zur Verwaltung der unternehmenseigenen Geräte in Intune stehen die folgenden Graph-Ressourcen zur Verfügung:

- [Profil für Active Directory Windows Autopilot Deployment](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [Profil für Azure AD Windows Autopilot Deployment](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [DEP-Registrierung – Basisprofil](intune-enrollment-depenrollmentbaseprofile.md)
- [DEP-Registrierungsprofil](intune-enrollment-depenrollmentprofile.md)
- [DEP iOS-Registrierungsprofil](intune-enrollment-depiosenrollmentprofile.md)
- [DEP macOS-Registrierungsprofil](intune-enrollment-depmacosenrollmentprofile.md)
- [DEP-Onboarding-Einstellung](intune-enrollment-deponboardingsetting.md)
- [DEP-Tokentyp](intune-enrollment-deptokentype.md)
- [Ermittlungsquelle](intune-enrollment-discoverysource.md)
- [Registrierungsprofil](intune-enrollment-enrollmentprofile.md)
- [Registrierungsstatus](intune-enrollment-enrollmentstate.md)
- [Importierte Apple-Geräteidentität](intune-enrollment-importedappledeviceidentity.md)
- [Ergebnis der importierten Apple-Geräteidentität](intune-enrollment-importedappledeviceidentityresult.md)
- [Importierte Geräteidentität](intune-enrollment-importeddeviceidentity.md)
- [Ergebnis der importierten Geräteidentität](intune-enrollment-importeddeviceidentityresult.md)
- [Typ der importierten Geräteidentität](intune-enrollment-importeddeviceidentitytype.md)
- [Importierte Windows Autopilot-Geräteidentität](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [Importstatus der importierten Windows Autopilot-Geräteidentität](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [Status der importierten Windows Autopilot-Geräteidentität](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [Upload der importierten Windows Autopilot-Geräteidentität](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [Uploadstatus der importierten Windows Autopilot-Geräteidentität](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [iTunes-Kopplungsmodus](intune-enrollment-itunespairingmode.md)
- [Verwaltungszertifikat mit Fingerabdruck](intune-enrollment-managementcertificatewiththumbprint.md)
- [Einstellungen für Windows-Willkommensseite](intune-enrollment-outofboxexperiencesettings.md)
- [Plattform](intune-enrollment-platform.md)
- [Profil für Windows Autopilot Deployment](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [Profilzuweisung für Windows Autopilot Deployment](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [Windows Autopilot-Geräteidentität](intune-enrollment-windowsautopilotdeviceidentity.md)
- [Windows Autopilot-Gerätetyp](intune-enrollment-windowsautopilotdevicetype.md)
- [Profil für Windows Autopilot – Detaillierter Zuweisungsstatus](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [Profil für Windows Autopilot – Zuweisungsstatus](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [Windows Autopilot-Einstellungen](intune-enrollment-windowsautopilotsettings.md)
- [Windows Autopilot-Synchronisierungsstatus](intune-enrollment-windowsautopilotsyncstatus.md)
- [Windows-Gerätenutzungstyp](intune-enrollment-windowsdeviceusagetype.md)
- [Bildschirmeinstellungen für Windows-Registrierungsstatus](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [Windows-Benutzertyp](intune-enrollment-windowsusertype.md)
