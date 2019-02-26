---
title: remoteaktions-Enumerationstyp
description: Remote Aktionen InTune unterstützt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4eb232f53ecb6b857e1a762ac0bef59c9ca246a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174874"
---
# <a name="remoteaction-enum-type"></a>remoteaktions-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Remote Aktionen InTune unterstützt.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Der Benutzer initiiert eine unbekannte Aktion.|
|factoryReset|1|Der Benutzer initiiert eine Aktion, um ein Gerät zurückzusetzen. |
|removeCompanyData|2|Der Benutzer initiiert eine Aktion zum Entfernen von Unternehmensdaten von einem Gerät. |
|resetPasscode|3|Der Benutzer initiiert eine Aktion zum Entfernen des Codes eines iOS-Geräts oder zum Zurücksetzen des Codes von Android/Windows-Gerät. |
|Remote Lock|4|Der Benutzer initiiert eine Aktion, um ein Gerät zu sperren.|
|enableLostMode|5|Der Benutzer initiiert eine Aktion, um den Verlust Modus auf einem überwachten iOS-Gerät zu aktivieren.|
|disableLostMode|6|Der Benutzer initiiert eine Aktion, um den Verlust Modus auf einem überwachten iOS-Gerät zu deaktivieren.|
|locateDevice|7|Der Benutzer initiiert eine Aktion zum Auffinden eines überwachten iOS-Geräts.|
|rebootNow|8|Der Benutzer initiiert eine Aktion zum Neustart eines Windows-Geräts.|
|recoverPasscode|9|Der Benutzer initiiert eine Aktion zum Zurücksetzen der PIN für Passport für die Arbeit auf dem Windows Phone-Gerät.|
|cleanWindowsDevice|10|Der Benutzer initiiert eine Aktion zum Bereinigen des Windows-Geräts.|
|logoutSharedAppleDeviceActiveUser|11|Der Benutzer initiiert eine Aktion zum Abmelden des aktuellen Benutzers auf einem freigegebenen Apple-Gerät.|
|quickScan|12|Der Benutzer initiiert eine Aktion zum Ausführen der Schnellsuche auf dem Gerät.|
|fullScan|13|Der Benutzer initiiert eine Aktion, um den vollständigen Scan auf dem Gerät auszuführen.|
|windowsDefenderUpdateSignatures|14|Der Benutzer initiiert eine Aktion zum Aktualisieren von Schadsoftware-Signaturen auf dem Gerät.|
|factoryResetKeepEnrollmentData|15|Der Benutzer initiiert ein Remote Zurücksetzungs Gerät für die Aktion, indem Registrierungsdaten beibehalten werden.|
|updateDeviceAccount|16|Der Benutzer initiiert eine Aktion zum Aktualisieren des Kontos auf dem Gerät.|
|automaticRedeployment|17|Der Benutzer initiiert eine Aktion zum automatischen erneuten Bereitstellen des Geräts|
|shutDown|18|Der Benutzer initiiert eine Aktion zum Herunterfahren des Geräts.|




