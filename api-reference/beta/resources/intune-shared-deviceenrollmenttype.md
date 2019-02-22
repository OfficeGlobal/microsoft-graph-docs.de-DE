---
title: deviceEnrollmentType-Enumerationstyp
description: Mögliche Möglichkeiten zum Hinzufügen eines mobilen Geräts zur Verwaltung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b186110c4f69ea7b6f4d12c9fb2a333927f81385
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173654"
---
# <a name="deviceenrollmenttype-enum-type"></a>deviceEnrollmentType-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Mögliche Möglichkeiten zum Hinzufügen eines mobilen Geräts zur Verwaltung.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Standardwert, der Registrierungstyp wurde nicht gesammelt.|
|userEnrollment|1|Benutzergesteuerte Registrierung über den BYOD-Kanal.|
|deviceEnrollmentManager|2|Benutzerregistrierung mit einem Geräte Registrierungs-Manager-Konto.|
|appleBulkWithUser|3|Apple Bulk Enrollment with User Challenge. (DEP, Apple Configurator)|
|appleBulkWithoutUser|4|Apple-Massenregistrierung ohne Benutzer Herausforderung. (DEP, Apple Configurator, Mobile Konfiguration)|
|windowsAzureADJoin|5|Windows 10 Azure AD Join.|
|windowsBulkUserless|6|Windows 10 Bulk-Registrierung über ICD mit Zertifikat.|
|windowsAutoEnrollment|7|Automatische Windows 10-Registrierung. (Arbeitskonto hinzufügen)|
|windowsBulkAzureDomainJoin|8|Windows 10 Bulk Azure AD Join.|
|windowsCoManagement|9|Durch autoPilot oder Gruppenrichtlinien ausgelöste Windows 10-Co-Verwaltung.|




