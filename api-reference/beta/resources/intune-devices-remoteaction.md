---
title: RemoteAction Enum-Typ
description: Remote Aktionen Intune unterstützt.
ms.openlocfilehash: 8ab503538edd1005106be9d30e67b35b6bb59583
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064238"
---
# <a name="remoteaction-enum-type"></a>RemoteAction Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Remote Aktionen Intune unterstützt.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Benutzer versucht, eine unbekannte Aktion.|
|factoryReset|1|Benutzer initiiert eine Aktion, die Factory Zurücksetzen eines Geräts. |
|removeCompanyData|2|Benutzer versucht, eine Aktion um Unternehmensdaten von einem Gerät zu entfernen. |
|resetPasscode|3|Benutzer versucht, eine Aktion, um die Kennung einer iOS-Gerät entfernen oder Zurücksetzen der Kennung von Android / Windows-Gerät. |
|remoteLock|4|Benutzer versucht, einer Aktion remote Sperren ein Geräts.|
|enableLostMode|5|Benutzer versucht, eine Aktion, um auf einem Gerät überwachten iOS verloren Modus aktivieren.|
|disableLostMode|6|Benutzer versucht, eine Aktion um verloren Modus auf einem überwachten iOS-Gerät zu deaktivieren.|
|locateDevice|7|Benutzer versucht, eine Aktion, um eine überwachten iOS-Geräte zu suchen.|
|rebootNow|8|Benutzer versucht, eine Aktion, um ein Windows-Gerät neu zu starten.|
|recoverPasscode|9|Benutzer versucht, eine Aktion, um die Pin für Passport für die Arbeit am Windows Phone-Gerät zurückzusetzen.|
|cleanWindowsDevice|10|Benutzer versucht, eine Aktion, um Windows-Gerät zu bereinigen.|
|logoutSharedAppleDeviceActiveUser|11|Benutzer versucht, eine Aktion zum aktuellen Benutzer auf freigegebene Apple Gerät abmelden.|
|quickScan|12|Benutzer versucht, eine Aktion, um schnell-Scan auf Gerät ausgeführt wird.|
|fullScan|13|Benutzer versucht, eine Aktion, um eine vollständige Überprüfung auf Gerät ausführen.|
|windowsDefenderUpdateSignatures|14|Benutzer versucht, eine Aktion um Malware Signaturen auf Gerät zu aktualisieren.|
|factoryResetKeepEnrollmentData|15|Benutzer versucht, eine Aktion Remotezurücksetzung Gerät mit dem Anmeldedaten beibehalten.|
|updateDeviceAccount|16|Benutzer versucht, eine Aktion um Konto auf Gerät zu aktualisieren.|
|automaticRedeployment|17|Benutzer versucht, eine Aktion Automatice Bereitstellen des Geräts|
|Herunterfahren|18|Benutzer versucht, eine Aktion, die das Gerät herunterfahren.|





