---
title: AndroidDeviceOwnerRequiredPasswordType Enum-Typ
description: Android-Gerät Besitzer Richtlinie erforderliche Kennworttyp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b1208de597baff9dd05a48663435a3a928f3dae9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938041"
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





