---
title: advancedBitLockerState-Enumerationstyp
description: Erweiterter BitLocker-Status
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8515f59b6fbba65f590b07c6a17fda55b4e9bd4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178143"
---
# <a name="advancedbitlockerstate-enum-type"></a>advancedBitLockerState-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Erweiterter BitLocker-Status

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|Erfolgreich|0|Erweiterter BitLocker-Status Erfolg|
|noUserConsent|1|Der Benutzer hat die Verschlüsselung nie erteilt.|
|osVolumeEncryptionMethodMismatch|2|Die Verschlüsselungsmethode des BS-Volumes unterscheidet sich von der Richtlinie|
|osVolumeTpmRequired|4|TPM wird nicht zum Schutz des Betriebssystem Volumens verwendet, ist jedoch für Richtlinien erforderlich|
|osVolumeTpmOnlyRequired|8|Nur TPM-Schutz, der nicht für das Betriebssystemvolume verwendet wird, aber für Richtlinien erforderlich ist|
|osVolumeTpmPinRequired|16|TPM + PIN-Schutz wird nicht für das Betriebssystemvolume verwendet, ist jedoch für Richtlinien erforderlich|
|osVolumeTpmStartupKeyRequired|32|TPM + Startschlüssel Schutz wird nicht für das Betriebssystemvolume verwendet, ist jedoch für Richtlinien erforderlich|
|osVolumeTpmPinStartupKeyRequired|64|TPM + PIN + Startschlüssel wird nicht für das Betriebssystemvolume verwendet, ist jedoch für Richtlinien erforderlich|
|osVolumeUnprotected|128|Das nicht geschützte Betriebssystem Volume wurde erkannt|
|recoveryKeyBackupFailed|256|Fehler bei der Sicherung des wiederHerstellungsschlüssels|
|fixedDriveNotEncrypted|512|Festplatte nicht verschlüsselt|
|fixedDriveEncryptionMethodMismatch|1024|Die Verschlüsselungsmethode eines fest Netzlaufwerks unterscheidet sich von der Richtlinie|
|loggedOnUserNonAdmin|2048|Der anGemeldete Benutzer ist nicht Administrator. Dies erfordert die Richtlinie "AllowStandardUserEncryption" auf 1 festgelegt.|
|windowsRecoveryEnvironmentNotConfigured|4096|WinRE ist nicht konfiguriert|
|tpmNotAvailable|8192|TPM ist für BitLocker nicht verfügbar. Dies bedeutet, dass TPM nicht vorhanden ist oder dass die nicht verfügbare TPM-Überschreibung festgelegt ist oder das Hostbetriebssystem auf Portable/Rome-able-Laufwerk|
|tpmNotReady|16384|TPM ist nicht für BitLocker bereit|
|networkError|32768|Netzwerk nicht verfügbar. Dies ist für die Wiederherstellungsschlüssel Sicherung erforderlich. Dies wird für Laufwerks Verschlüsselungs fähige Geräte gemeldet.|




