---
title: DeviceEnrollmentFailureReason Enum-Typ
description: Oberste Ebene Fehler Kategorien für die Registrierung.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fbfe7193c72f1ff1a03a7e7bb4da57d0a032e530
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396210"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>DeviceEnrollmentFailureReason Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Oberste Ebene Fehler Kategorien für die Registrierung.

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Der Standardwert, Fehlerursache ist unbekannt.|
|Authentifizierung|1|Fehler bei der Authentifizierung|
|Autorisierung|2|Anruf wurde authentifiziert, jedoch nicht autorisiert, registrieren.|
|accountValidation|3|Fehler beim Überprüfen von des Kontos für die Registrierung. (Konto blockiert, Registrierung nicht aktiviert)|
|userValidation|4|Benutzer konnte nicht überprüft werden. (Benutzer ist nicht vorhanden, fehlende Lizenz)|
|deviceNotSupported|5|Gerät ist nicht für die Verwaltung von mobilen Geräten unterstützt.|
|inMaintenance|6|Konto ist in der Wartung.|
|badRequest|7|Client gesendet eine Anforderung, die nicht vom Dienst verstanden/unterstützt wird.|
|featureNotSupported|8|Features, die durch diese Registrierung verwendet werden für dieses Konto nicht unterstützt.|
|enrollmentRestrictionsEnforced|9|Registrierung Einschränkungen durch den Administrator konfiguriert blockiert diese Registrierung.|
|clientDisconnected|10|Client ein Timeout aufgetreten, oder die Registrierung mithilfe des Endbenutzers abgebrochen wurde.|
|userAbandonment|11|Registrierung wurde abgebrochen, mithilfe des Endbenutzers. (Des Endbenutzers Onboarding gestartet, aber nicht in kurzer Zeit abgeschlossen)|




