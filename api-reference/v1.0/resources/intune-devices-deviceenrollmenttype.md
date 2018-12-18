---
title: DeviceEnrollmentType Enum-Typ
description: Mögliche Methoden zum Hinzufügen eines mobilen Geräts zu Management.
author: tfitzmac
ms.openlocfilehash: db66ca30758c11230282f7f3a1f6966089d6883b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339326"
---
# <a name="deviceenrollmenttype-enum-type"></a>DeviceEnrollmentType Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Methoden zum Hinzufügen eines mobilen Geräts zu Management.
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
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



