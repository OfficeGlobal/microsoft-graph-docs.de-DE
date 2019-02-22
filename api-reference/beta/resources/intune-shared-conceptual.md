---
title: FreigeGebene Ressourcen in Microsoft InTune – Microsoft Graph-API
description: Listet die Microsoft Graph-API für InTune-Endpunkte (REST) auf, die mehrere Workflows für eine mandantenorganisation unterstützen.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 6436f134ae9e95623b073f6e645f0737d45d540e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158310"
---
# <a name="shared-resources-in-microsoft-intune"></a>FreigeGebene Ressourcen in Microsoft InTune

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.

Diese Endpunkte werden in mehreren Microsoft Graph-APIs für InTune-Workflows verwendet.  Die Absicht, der Zweck und die Berechtigungen, die für die Verwendung einer bestimmten Ressource erforderlich sind, hängen vom jeweiligen Workflow und Kontext des zugrunde liegenden Aufrufs ab.  Darüber hinaus werden bestimmte Methoden, Eigenschaften und Aktionen nur für bestimmte Workflows unterstützt.

Die folgenden Graph-Ressourcen werden zwischen InTune-Workflows gemeinsam genutzt:

- [Aktionszustand](intune-shared-actionstate.md)
- [allDevicesAssignmentTarget](intune-shared-alldevicesassignmenttarget.md)
- [allLicensedUsersAssignmentTarget](intune-shared-alllicensedusersassignmenttarget.md)
- [Compliance-Status](intune-shared-compliancestatus.md)
- [deviceAndAppManagementAssignmentTarget](intune-shared-deviceandappmanagementassignmenttarget.md)
- [Geräte-App-Verwaltung](intune-shared-deviceappmanagement.md)
- [Gerätekategorie](intune-shared-devicecategory.md)
- [Geräteregistrierungstyp](intune-shared-deviceenrollmenttype.md)
- [deviceManagement](intune-shared-devicemanagement.md)
- [Geräteplattformtyp](intune-shared-deviceplatformtype.md)
- [Gerätetyp](intune-shared-devicetype.md)
- [Aktivierung](intune-shared-enablement.md)
- [exclusionGroupAssignmentTarget](intune-shared-exclusiongroupassignmenttarget.md)
- [groupAssignmentTarget](intune-shared-groupassignmenttarget.md)
- [Installationsabsicht](intune-shared-installintent.md)
- [ipRange](intune-shared-iprange.md)
- [iPv4Range](intune-shared-ipv4range.md)
- [iPv6Range](intune-shared-ipv6range.md)
- [keyValuePair](intune-shared-keyvaluepair.md)
- [MIME-Inhalt](intune-shared-mimecontent.md)
- [Mobile App – Problembehandlung – Ereignis](intune-shared-mobileapptroubleshootingevent.md)
- [proxiedDomain](intune-shared-proxieddomain.md)
- [Report](intune-shared-report.md)
- [reportRoot](intune-shared-reportroot.md)
- [Resultierender App-Status](intune-shared-resultantappstate.md)
- [RGB-Farbe](intune-shared-rgbcolor.md)
- [Kontotyp „Ausführen als“](intune-shared-runasaccounttype.md)
- [Ausführungsstatus](intune-shared-runstate.md)
- [Gespeicherte Optionen für Generierung des Benutzeroberflächenzustands](intune-shared-saveduistategenerationoptions.md)
- [URI](intune-shared-uri.md)
- [Benutzer](intune-shared-user.md)
- [Kontotyp des VPP-Tokens](intune-shared-vpptokenaccounttype.md)
- [Fehlerursache für VPP-Tokenaktion](intune-shared-vpptokenactionfailurereason.md)
- [Konfiguration für Windows-Domänenbeitritt](intune-shared-windowsdomainjoinconfiguration.md)
