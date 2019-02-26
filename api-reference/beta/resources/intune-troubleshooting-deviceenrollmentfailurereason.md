---
title: deviceEnrollmentFailureReason-Enumerationstyp
description: Kategorien für die Registrierung auf höchster Ebene
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f03ce73f1d6f8b5edc6b3e3b661f9a7ba79407bb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163854"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>deviceEnrollmentFailureReason-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

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




