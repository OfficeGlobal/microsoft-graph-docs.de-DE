---
title: AndroidDeviceOwnerRequiredPasswordType Enum-Typ
description: Android-Gerät Besitzer Richtlinie erforderliche Kennworttyp.
author: tfitzmac
ms.openlocfilehash: e0903bbf5720350b35bf7e5fe5c9a5f9584810c1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330226"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>AndroidDeviceOwnerRequiredPasswordType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Android-Gerät Besitzer Richtlinie erforderliche Kennworttyp.
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Gerät Standardwert, keine beabsichtigt.|
|erforderlich|1|Es muss ein Kennwort festlegen, jedoch ohne Einschränkungen auf Typ.|
|numerische|2|AT mindestens numerische.|
|numericComplex|3|AT mindestens numerische mit keine wiederholten oder eine geordneten Sequenzen.|
|Alphabetische|4|Mindestens alphabetische Kennwort.|
|Alphanumerisch|5|Mindestens Alphanumerisches Kennwort|
|alphanumericWithSymbols|6|Mindestens alphanumerische durch Geviertstrich.|





