---
title: windowsPrivacyDataCategory-Enumerationstyp
description: Windows-Datenschutzkategorie-Spezifizierer für Datenschutz.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3097ed916ec9f215880caf46bcdc02616ce5d2c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154453"
---
# <a name="windowsprivacydatacategory-enum-type"></a>windowsPrivacyDataCategory-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Windows-Datenschutzkategorie-Spezifizierer für Datenschutz.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|notConfigured|0|Keine Zugriffsebene angegeben, keine Absichten. Das Gerät kann sich entweder wie in UserInControl oder in ForceAllow Verhalten. Es kann davon abhängen, auf welche Daten auf dem Datenschutz zugegriffen wurde, wie Windows-Versionen und andere Faktoren.|
|accountInfo|1|Apps können auf den Namen des Benutzers, Bild und andere Kontoinformationen zugreifen, die in Microsoft-Konto erstellt wurden. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|appsRunInBackground|2|Zulassen, dass apps Informationen empfangen, Benachrichtigungen senden und auf dem neuesten Stand bleiben, auch wenn der Benutzer Sie nicht verwendet. Beachten Sie, dass bei der Deaktivierung von Kommunikations-Apps (E-Mail, Sprachausgabe usw.) aus dem Hintergrund Zugriff diese apps möglicherweise nicht wie beim Hintergrund Zugriff funktionieren. HinzugeFügt in Windows 10, Version 1703.|
|calendar|3|Apps können auf den Kalender des Benutzers zugreifen. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|callHistory|4|Apps können auf den Anrufverlauf von Benutzern zugreifen. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|Kamera|5|Apps können auf dem Gerät des Benutzers auf die Kamera zugreifen. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|contacts|6|Apps können auf die Kontaktinformationen des Benutzers zugreifen. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|diagnosticsInfo|7|Apps können auf Diagnoseinformationen zu anderen laufenden apps zugreifen. HinzugeFügt in Windows 10, Version 1703.|
|email|8|Apps können auf e-Mail zugreifen und e-Mails senden. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|location|9|Apps können auf die genauen Standortdaten des Geräte Benutzers zugreifen. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|Messaging|10|Apps können Nachrichten, Text oder MMS lesen oder senden. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|microphone|11|Lassen Sie die apps Mikrofon auf dem Benutzergerät verwenden. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|Bewegung|12|Apps verwenden Bewegungsdaten, die auf dem Geräte Benutzer generiert werden. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|Benachrichtigungen|13|Apps können auf Benutzer Benachrichtigungen zugreifen. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|phone|14|Apps können auf Telefondaten zugreifen und telefonieren. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|Radios|15|Lassen Sie apps Funkgeräte, einschließlich Bluetooth, zum Senden und empfangen von Daten verwenden. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|tasks|16|Apps können auf die Aufgabenplanung zugreifen. HinzugeFügt in Windows 10, Version 1703.|
|syncWithDevices|17|Lassen Sie Apps automatisch Informationen mit Drahtlosgeräten freigeben und synchronisieren, die nicht explizit mit dem Benutzergerät verbunden sind. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|trustedDevices|18|Apps können auf vertrauenswürdige Geräte zugreifen. Dies wurde in Windows 10, Version 1607, hinzugefügt.|




