---
title: Unternehmenseigene Geräte mit Intune registrieren
description: " Szenario (BYOD)."
ms.openlocfilehash: b6c498a1471b95f28c26fb035eec3349108e1ec3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064231"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a>Unternehmenseigene Geräte mit Intune registrieren

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.

Sie können organisations- oder unternehmenseigene Geräte für die Verwaltung in Intune auf unterschiedliche Weise und abhängig von der Art des Geräts, der Art der Anschaffung des Geräts und den Anforderungen der Organisation registrieren. Sie können auch die Unternehmensportal-App installieren, um unternehmenseigene Geräte zu registrieren und verwalten, wie z. B. in einem Szenario mit geschäftlich genutzten Privatgeräten der Benutzer (BYOD).

Zur Verwaltung der unternehmenseigenen Geräte in Intune stehen die folgenden Graph-Ressourcen zur Verfügung:

- [Active Directory Windows Autopilot Bereitstellung Benutzerprofil](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [Azure AD Windows Autopilot Bereitstellung Benutzerprofil](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [Datenausführungsverhinderung Registrierung Profil](intune-enrollment-depenrollmentbaseprofile.md)
- [Datenausführungsverhinderung Registrierung Profil](intune-enrollment-depenrollmentprofile.md)
- [Datenausführungsverhinderung iOS Registrierung Profil](intune-enrollment-depiosenrollmentprofile.md)
- [Datenausführungsverhinderung Mac OS Registrierung Profil](intune-enrollment-depmacosenrollmentprofile.md)
- [DEP auf mittels Fingereingabe-Einstellung](intune-enrollment-deponboardingsetting.md)
- [Datenausführungsverhinderung token-Typ](intune-enrollment-deptokentype.md)
- [Discovery-Quelle](intune-enrollment-discoverysource.md)
- [Registrierung Profil](intune-enrollment-enrollmentprofile.md)
- [Status der Registrierung](intune-enrollment-enrollmentstate.md)
- [Importierte Apple Gerät Identität](intune-enrollment-importedappledeviceidentity.md)
- [Apple Gerät Identität Ergebnis importiert](intune-enrollment-importedappledeviceidentityresult.md)
- [Importierte Gerät Identität](intune-enrollment-importeddeviceidentity.md)
- [Importiert Gerät Identität Ergebnis](intune-enrollment-importeddeviceidentityresult.md)
- [Gerätetyp Identität importiert](intune-enrollment-importeddeviceidentitytype.md)
- [Importierte Windows Autopilot Gerät Identität](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [Importierte Windows Autopilot Identität Import Gerätestatus](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [Importierte Windows Identity Autopilot Gerätestatus](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [Importierte Windows Autopilot Gerät Identität hochladen](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [Importierte Windows Autopilot Identität Upload Gerätestatus](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [iTunes paarungs-Modus](intune-enrollment-itunespairingmode.md)
- [Management-Zertifikat mit dem Fingerabdruck](intune-enrollment-managementcertificatewiththumbprint.md)
- [Erleben Sie die Einstellungen im Lieferzustand](intune-enrollment-outofboxexperiencesettings.md)
- [Plattform](intune-enrollment-platform.md)
- [Windows Autopilot Bereitstellung Benutzerprofil](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [Windows Autopilot Bereitstellung Profil Zuordnung](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [Windows Autopilot Gerät Identität](intune-enrollment-windowsautopilotdeviceidentity.md)
- [Windows Autopilot Profil Zuordnung detaillierter status](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [Zuordnung des Status von Windows Autopilot Profil](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [Windows Autopilot-Einstellungen](intune-enrollment-windowsautopilotsettings.md)
- [Windows Autopilot Synchronisierungsstatus](intune-enrollment-windowsautopilotsyncstatus.md)
- [Windows-Gerät Verwendungstyp](intune-enrollment-windowsdeviceusagetype.md)
- [Windows-Registrierung Status Bildschirm-Einstellungen](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [Windows-Benutzertyp](intune-enrollment-windowsusertype.md)
