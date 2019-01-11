---
title: Registrieren von Geräten für die Verwaltung in Intune
description: " Registrierung (BYOD) kann Benutzer ihre persönliche Telefone, Tablets oder PCs zu registrieren. Die Registrierung unternehmenseigener Geräte (COD) ermöglicht Verwaltungsszenarien wie Remotezurücksetzung, gemeinsam genutzte Geräte oder Benutzeraffinität für ein Gerät."
localization_priority: Normal
ms.openlocfilehash: de2a87c08851081891ee641db50a4ca1c64cb314
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841321"
---
# <a name="enroll-devices-for-management-in-intune"></a>Registrieren von Geräten für die Verwaltung in Intune

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.

Sie können Geräte wie z. B. Windows-PCs registrieren, um die Verwaltung mobiler Geräte (MDM) mit Microsoft Intune zu ermöglichen. In diesem Thema werden verschiedene Methoden für die Registrierung mobiler Geräte für die Verwaltung in Intune beschrieben. Die Art der Registrierung hängt vom Gerätetyp, der Eigentümerschaft und dem erforderlichen Verwaltungsgrad ab. Bei der „Bring your own device“ (BYOD)-Registrierung können Benutzer ihre eigenen Smartphones, Tablets oder PCs registrieren. Die Registrierung unternehmenseigener Geräte (COD) ermöglicht Verwaltungsszenarien wie Remotezurücksetzung, gemeinsam genutzte Geräte oder Benutzeraffinität für ein Gerät.

Die folgenden Graph-Ressourcen stehen für die Registrierungsverwaltung in Intune zur Verfügung:  

- [Konfiguration der Geräteregistrierung](intune-onboarding-deviceenrollmentconfiguration.md)
- [Konfiguration der Geräteregistrierungsgrenze](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [Geräteregistrierung – Plattformeinschränkung](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [Konfiguration der Plattformeinschränkungen für Geräteregistrierung](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [Geräteregistrierung – Windows Hello für Business-Konfiguration](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [Exchange Connector für Geräteverwaltung](intune-onboarding-devicemanagementexchangeconnector.md)
- [Verwaltung von Exchange Connector Gerätestatus](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [Verwaltung von Exchange Connector Sync Gerätetyp](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [Verwaltung von Exchange Connector Gerätetyp](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [Geräteverwaltungspartner](intune-onboarding-devicemanagementpartner.md)
- [Gerät Management Partner app-Typ](intune-onboarding-devicemanagementpartnerapptype.md)
- [Management Partner Mandanten Gerätestatus](intune-onboarding-devicemanagementpartnertenantstate.md)
- [Aktivierung von Steuerelementen](intune-onboarding-enablement.md)
- [Zuweisung der Registrierungskonfiguration](intune-onboarding-enrollmentconfigurationassignment.md)
- [Intune-Marke](intune-onboarding-intunebrand.md)
- [MDM Autorität](intune-onboarding-mdmauthority.md)
- [MTD-Connector (Mobile Threat Defense)](intune-onboarding-mobilethreatdefenseconnector.md)
- [Mobile Bedrohung Partner Mandanten Zustand](intune-onboarding-mobilethreatpartnertenantstate.md)
- [Einstellungen für lokalen, bedingten Zugriff](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [Organisation](intune-onboarding-organization.md)
- [RGB-Farbe](intune-onboarding-rgbcolor.md)
- [VPP token](intune-onboarding-vpptoken.md)
- [VPP token Zustand](intune-onboarding-vpptokenstate.md)
- [VPP token Synchronisierungsstatus](intune-onboarding-vpptokensyncstatus.md)
- [Windows Hello für die Verwendung der Business-PIN](intune-onboarding-windowshelloforbusinesspinusage.md)
