---
title: Integrierte verwaltete Geräte mit InTune – Microsoft Graph-API
description: Listet die Microsoft Graph-API für InTune-Endpunkte (REST) auf, die zum Onboarding (configure and initialize) Devices for a Mandanten Organization verwendet werden.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 2acd4310c07fd1532a1a16bdc419d7bad23bc973
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147831"
---
# <a name="enroll-devices-for-management-in-intune"></a>Registrieren von Geräten für die Verwaltung in Intune

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.

Sie können Geräte wie z. B. Windows-PCs registrieren, um die Verwaltung mobiler Geräte (MDM) mit Microsoft Intune zu ermöglichen. In diesem Thema werden verschiedene Methoden für die Registrierung mobiler Geräte für die Verwaltung in Intune beschrieben. Die Art der Registrierung hängt vom Gerätetyp, der Eigentümerschaft und dem erforderlichen Verwaltungsgrad ab. Bei der „Bring your own device“ (BYOD)-Registrierung können Benutzer ihre eigenen Smartphones, Tablets oder PCs registrieren. Die Registrierung unternehmenseigener Geräte (COD) ermöglicht Verwaltungsszenarien wie Remotezurücksetzung, gemeinsam genutzte Geräte oder Benutzeraffinität für ein Gerät.

Die folgenden Graph-Ressourcen stehen für die Registrierungsverwaltung in Intune zur Verfügung:

- [Certificate Connector-Einstellung](intune-onboarding-certificateconnectorsetting.md)
- [Geräte- und App-Verwaltungsdaten](intune-onboarding-deviceandappmanagementdata.md)
- [Konfiguration der Geräteregistrierung](intune-onboarding-deviceenrollmentconfiguration.md)
- [Konfiguration der Geräteregistrierungsgrenze](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [Geräteregistrierung – Plattformeinschränkung](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [Konfiguration der Plattformeinschränkungen für Geräteregistrierung](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [Geräteregistrierung – Windows Hello für Business-Konfiguration](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [Exchange-Zugriffsebene für Geräteverwaltung](intune-onboarding-devicemanagementexchangeaccesslevel.md)
- [Exchange-Zugriffsregel für Geräteverwaltung](intune-onboarding-devicemanagementexchangeaccessrule.md)
- [Exchange-Zugriffsregeltyp für Geräteverwaltung](intune-onboarding-devicemanagementexchangeaccessruletype.md)
- [Exchange Connector für Geräteverwaltung](intune-onboarding-devicemanagementexchangeconnector.md)
- [Status des Exchange Connectors für Geräteverwaltung](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [Synchronisierungstyp des Exchange Connectors für Geräteverwaltung](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [Typ des Exchange Connectors für Geräteverwaltung](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [Exchange-Geräteklasse für Geräteverwaltung](intune-onboarding-devicemanagementexchangedeviceclass.md)
- [Richtlinie von lokalem Exchange für Geräteverwaltung](intune-onboarding-devicemanagementexchangeonpremisespolicy.md)
- [Geräteverwaltungspartner](intune-onboarding-devicemanagementpartner.md)
- [App-Typ für Geräteverwaltungspartner](intune-onboarding-devicemanagementpartnerapptype.md)
- [Mandantenstatus für Geräteverwaltungspartner](intune-onboarding-devicemanagementpartnertenantstate.md)
- [Zuweisung der Registrierungskonfiguration](intune-onboarding-enrollmentconfigurationassignment.md)
- [Intune-Marke](intune-onboarding-intunebrand.md)
- [MDM-Zertifizierungsstelle](intune-onboarding-mdmauthority.md)
- [Microsoft Store für Business-Portal – Auswahloptionen](intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)
- [MTD-Connector (Mobile Threat Defense)](intune-onboarding-mobilethreatdefenseconnector.md)
- [Mandantenstatus für Mobile Threat-Partner](intune-onboarding-mobilethreatpartnertenantstate.md)
- [Einstellungen für lokalen, bedingten Zugriff](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [Organisation](intune-onboarding-organization.md)
- [Querladeschlüssel](intune-onboarding-sideloadingkey.md)
- [VPP-Token](intune-onboarding-vpptoken.md)
- [VPP-Token – Aktionsergebnis](intune-onboarding-vpptokenactionresult.md)
- [VPP-Token – Lizenzzusammenfassung](intune-onboarding-vpptokenlicensesummary.md)
- [VPP-Token – Lizenzen widerrufen – Aktionsergebnis](intune-onboarding-vpptokenrevokelicensesactionresult.md)
- [VPP-Tokenstatus](intune-onboarding-vpptokenstate.md)
- [Synchronisierungsstatus des VPP-Tokens](intune-onboarding-vpptokensyncstatus.md)
- [Konfiguration der Fertigstellungsseite der Windows 10-Registrierung](intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)
- [PIN-Verwendung für Windows Hello for Business ](intune-onboarding-windowshelloforbusinesspinusage.md)
