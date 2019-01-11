---
title: DeviceEnrollmentFailureReason Enum-Typ
description: Oberste Ebene Fehler Kategorien für die Registrierung.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5dd7ba949c95d507d956dd7f315b3c19e0759c20
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885526"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>DeviceEnrollmentFailureReason Enum-Typ

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


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->
