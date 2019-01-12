---
title: DeviceEnrollmentType Enum-Typ
description: Mögliche Methoden zum Hinzufügen eines mobilen Geräts zu Management.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 72acbdf412ebb91269fcdc3f851ffbc204e0274b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987755"
---
# <a name="deviceenrollmenttype-enum-type"></a>DeviceEnrollmentType Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Methoden zum Hinzufügen eines mobilen Geräts zu Management.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Standardwert, Registrierung Typ wurde nicht aufgelistet.|
|userEnrollment|1|Benutzer gesteuerten Registrierung über BYOD Kanal.|
|deviceEnrollmentManager|2|Registrierung der Benutzer mit einem Gerät Registrierungs-Manager-Konto.|
|appleBulkWithUser|3|Apple Bulk Registrierung mit dem Benutzer Herausforderung (DEP, Apple-Konfiguration).|
|appleBulkWithoutUser|4|Apple Bulk Registrierung ohne Benutzer Herausforderung (DEP Apple-Konfiguration, Mobile Config).|
|windowsAzureADJoin|5|Windows Azure AD 10 teilnehmen.|
|windowsBulkUserless|6|Windows 10 Bulk Registrierung über ICD mit dem Zertifikat.|
|windowsAutoEnrollment|7|Automatische 10 Windows-Registrierung. (Arbeit Konto hinzufügen)|
|windowsBulkAzureDomainJoin|8|Massen-10 Windows Azure AD teilnehmen.|
|windowsCoManagement|9|Windows 10 gemeinsame Verwaltung durch AutoPilot oder Gruppenrichtlinien ausgelöst.|



