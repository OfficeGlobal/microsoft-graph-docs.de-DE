---
title: androidDeviceOwnerRequiredPasswordType-Enumerationstyp
description: Android-Gerätebesitzer Richtlinie erforderlicher Kennworttyp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 79d71fbabc4597c87c9cee782904334e2f12d7e8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172590"
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
|Alphanumerisch|5|Mindestens alphanumerisches Kennwort|
|alphanumericWithSymbols|6|Mindestens alphanumerisch mit Symbolen.|




