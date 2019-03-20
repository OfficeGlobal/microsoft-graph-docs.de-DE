---
title: androidDeviceOwnerRequiredPasswordType-Enumerationstyp
description: Android-Gerätebesitzer Richtlinie erforderlicher Kennworttyp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 376e33edac921f6771d76a45622a58bca3076c5c
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572334"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>androidDeviceOwnerRequiredPasswordType-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Android-Gerätebesitzer Richtlinie erforderlicher Kennworttyp.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Geräte-Standardwert, keine Absicht.|
|erforderlich|1|Es muss ein Kennwort festgelegt sein, es gibt jedoch keine Einschränkungen für den Typ.|
|numerischen|2|Mindestens numerisch.|
|numericComplex|3|Mindestens eine numerische ohne Wiederhol-oder geordnete Sequenzen.|
|alphabetischer|4|Mindestens ein alphabetisches Kennwort.|
|Alpha|5|Mindestens alphanumerisches Kennwort|
|alphanumericWithSymbols|6|Mindestens alphanumerisch mit Symbolen.|
|lowSecurityBiometric|7|Niedriges Biometrie-basiertes Kennwort erforderlich.|




