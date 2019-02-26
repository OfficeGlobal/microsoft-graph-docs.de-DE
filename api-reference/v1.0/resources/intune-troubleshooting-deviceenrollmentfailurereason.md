---
title: deviceEnrollmentFailureReason-Enumerationstyp
description: Kategorien für die Registrierung auf höchster Ebene
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 623030bccfac9e023a0d1df2dff7ea317b503485
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258331"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>deviceEnrollmentFailureReason-Enumerationstyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Kategorien für die Registrierung auf höchster Ebene

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Standardwert: der Ausfallgrund ist unbekannt.|
|Authentifizierung|1|Authentifizierung fehlgeschlagen|
|Autorisierung|2|Der Anruf wurde authentifiziert, aber nicht zur Registrierung autorisiert.|
|accountValidation|3|Fehler beim Überprüfen des Kontos für die Registrierung. (Konto gesperrt, Registrierung nicht aktiviert)|
|userValidation|4|Der Benutzer konnte nicht validiert werden. (Benutzer ist nicht vorhanden, fehlende Lizenz)|
|deviceNotSupported|5|Das Gerät wird für die Verwaltung mobiler Geräte nicht unterstützt.|
|inMaintenance|6|Das Konto ist in Wartung.|
|badRequest|7|Der Client hat eine Anforderung gesendet, die vom Dienst nicht verstanden/unterstützt wird.|
|featureNotSupported|8|Von dieser Registrierung verwendete Features werden für dieses Konto nicht unterstützt.|
|enrollmentRestrictionsEnforced|9|Durch den Administrator konfigurierte Registrierungs Einschränkungen haben diese Registrierung blockiert.|
|clientDisconnected|10|Timeout des Clients, oder die Registrierung wurde vom Endverbraucher abgebrochen.|
|userAbandonment|11|Die Registrierung wurde vom Endverbraucher abgebrochen. (Der Endanwender hat das Onboarding gestartet, konnte es jedoch nicht rechtzeitig abschließen)|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->

