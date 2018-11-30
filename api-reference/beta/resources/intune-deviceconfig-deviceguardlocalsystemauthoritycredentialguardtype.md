---
title: DeviceGuardLocalSystemAuthorityCredentialGuardType Enum-Typ
description: Mögliche Werte von Anmeldeinformationen Guard-Einstellungen.
ms.openlocfilehash: 73668ec4d6d5026402757fae3443da4540fb374c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058190"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a>DeviceGuardLocalSystemAuthorityCredentialGuardType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte von Anmeldeinformationen Guard-Einstellungen.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|nicht konfiguriert|0|Schaltet Anmeldeinformationen Guard Remote Wenn zuvor ohne UEFI Sperre konfiguriert.|
|enableWithUEFILock|1|Aktiviert die Anmeldeinformationen Guard mit UEFI sperren.|
|enableWithoutUEFILock|2|Aktiviert die Anmeldeinformationen Guard ohne UEFI sperren.|





