---
title: AndroidDeviceOwnerRequiredPasswordType Enum-Typ
description: Android-Gerät Besitzer Richtlinie erforderliche Kennworttyp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c53cc67d01886b76a20eef149a59c1d1fef4fc83
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887647"
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





