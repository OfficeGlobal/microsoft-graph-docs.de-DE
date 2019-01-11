---
title: WindowsPrivacyDataCategory Enum-Typ
description: Windows private Daten Kategorie Bezeichner für den Datenschutz Datenzugriff.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f9b533b9ecbf08f09760b57bb0d2bac7080746e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826752"
---
# <a name="windowsprivacydatacategory-enum-type"></a>WindowsPrivacyDataCategory Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Windows private Daten Kategorie Bezeichner für den Datenschutz Datenzugriff.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|nicht konfiguriert|0|Keine Zugriffsebene angegeben, keine Intents. Gerät kann entweder wie in UserInControl oder ForceAllow Verhalten. Es kann die private Daten abhängen wurde Zugriff auf Windows-Versionen und anderen Faktoren.|
|Kontostatus|1|Lassen Sie apps Zugriff Benutzernamen ein, Bild und andere Kontoinformationen in Microsoft-Konto erstellt. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|appsRunInBackground|2|Zulassen Sie der apps erhalten Informationen, Benachrichtigungen senden, und kommunizieren von Unternehmensinformationen Sie aktuellen, wenn der Benutzer nicht verwendet werden. Beachten Sie, dass bei der Kommunikation apps (E-Mail, Voicemail, usw.) aus Hintergrund Zugriff deaktivieren diese apps können oder nicht funktioniert, wie sie mit dem Hintergrund Zugriff sind. In Windows 10, Version 1703 hinzugefügt.|
|Kalender|3|Lassen Sie apps Access Benutzer Kalenders. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|callHistory|4|Lassen Sie Anrufliste apps zugreifen auf Benutzer. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|Kamera|5|Können Sie apps, die die Kamera auf das Gerät des Benutzers zugreifen. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|contacts|6|Lassen Sie die Kontaktinformationen apps zugreifen auf Benutzer. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|diagnosticsInfo|7|Können Sie apps, die Diagnoseinformationen zu anderen ausgeführten apps zugreifen. In Windows 10, Version 1703 hinzugefügt.|
|E-Mail|8|Lassen Sie apps Access und senden Sie e-Mail. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|location|9|Können Sie apps, die genaue Speicherort Daten des Benutzers Gerät zugreifen. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|Messaging|10|Lassen Sie apps lesen oder Senden von Nachrichten, Text oder MMS. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|microphone|11|Können Sie apps, die auf dem Benutzergerät Mikrofon verwenden. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|Bewegung|12|Können Sie apps Motion-Daten auf den Benutzer des Geräts generiert verwenden. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|Benachrichtigungen|13|Lassen Sie Benachrichtigungen apps zugreifen auf Benutzer. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|phone|14|Lassen Sie apps Access Daten Telefon und tätigen von Telefonanrufen. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|Sender|15|Können Sie apps Sender, einschließlich Bluetooth, senden und Empfangen von Daten verwenden. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|tasks|16|Let apps Zugriff Taskplaner. In Windows 10, Version 1703 hinzugefügt.|
|syncWithDevices|17|Können Sie apps, automatisch freigeben und Info mit drahtlosen Geräten, die explizit mit Gerät des Benutzers ein nicht synchronisieren. Dies wurde in Windows 10, Version 1607, hinzugefügt.|
|trustedDevices|18|Können Sie apps, die vertrauenswürdige Geräte zugreifen. Dies wurde in Windows 10, Version 1607, hinzugefügt.|





