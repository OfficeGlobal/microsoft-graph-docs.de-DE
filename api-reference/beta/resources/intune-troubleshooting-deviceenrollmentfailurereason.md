---
title: DeviceEnrollmentFailureReason Enum-Typ
description: Oberste Ebene Fehler Kategorien für die Registrierung.
ms.openlocfilehash: c0062a829811d9fb25453adb260d4d2be0295dd7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064467"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>DeviceEnrollmentFailureReason Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Oberste Ebene Fehler Kategorien für die Registrierung.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
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





