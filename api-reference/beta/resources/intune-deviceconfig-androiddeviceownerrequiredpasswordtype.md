---
title: AndroidDeviceOwnerRequiredPasswordType Enum-Typ
description: Android-Gerät Besitzer Richtlinie erforderliche Kennworttyp.
ms.openlocfilehash: 16f4bc59f2b4fa9f37989d1bc1978cdfacb2892c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062553"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>AndroidDeviceOwnerRequiredPasswordType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Android-Gerät Besitzer Richtlinie erforderliche Kennworttyp.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Gerät Standardwert, keine beabsichtigt.|
|erforderlich|1|Es muss ein Kennwort festlegen, jedoch ohne Einschränkungen auf Typ.|
|numerische|2|AT mindestens numerische.|
|numericComplex|3|AT mindestens numerische mit keine wiederholten oder eine geordneten Sequenzen.|
|Alphabetische|4|Mindestens alphabetische Kennwort.|
|Alphanumerisch|5|Mindestens Alphanumerisches Kennwort|
|alphanumericWithSymbols|6|Mindestens alphanumerische durch Geviertstrich.|





