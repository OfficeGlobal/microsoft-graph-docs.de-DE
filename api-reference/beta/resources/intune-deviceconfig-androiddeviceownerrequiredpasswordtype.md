---
title: AndroidDeviceOwnerRequiredPasswordType Enum-Typ
description: Android-Gerät Besitzer Richtlinie erforderliche Kennworttyp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c405cf3a69597994d5539427698baa92cabd3904
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403539"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>AndroidDeviceOwnerRequiredPasswordType Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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




