---
title: DeviceEnrollmentType Enum-Typ
description: Mögliche Methoden zum Hinzufügen eines mobilen Geräts zu Management.
ms.openlocfilehash: adee8eec9908953ab82268e19cf95edfb67ecc39
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063555"
---
# <a name="deviceenrollmenttype-enum-type"></a>DeviceEnrollmentType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Methoden zum Hinzufügen eines mobilen Geräts zu Management.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Standardwert, Registrierung Typ wurde nicht aufgelistet.|
|userEnrollment|1|Benutzer gesteuerten Registrierung über BYOD Kanal.|
|deviceEnrollmentManager|2|Registrierung der Benutzer mit einem Gerät Registrierungs-Manager-Konto.|
|appleBulkWithUser|3|Apple Bulk Registrierung mit dem Benutzer Herausforderung. (DEP, Apple-Konfiguration)|
|appleBulkWithoutUser|4|Apple Bulk Registrierung ohne Benutzer Herausforderung. (Mobile Config DEP Apple-Konfiguration)|
|windowsAzureADJoin|5|Windows Azure AD 10 teilnehmen.|
|windowsBulkUserless|6|Windows 10 Bulk Registrierung über ICD mit dem Zertifikat.|
|windowsAutoEnrollment|7|Automatische 10 Windows-Registrierung. (Arbeit Konto hinzufügen)|
|windowsBulkAzureDomainJoin|8|Massen-10 Windows Azure AD teilnehmen.|
|windowsCoManagement|9|Windows 10 Co-Management durch AutoPilot oder Gruppenrichtlinien ausgelöst.|




