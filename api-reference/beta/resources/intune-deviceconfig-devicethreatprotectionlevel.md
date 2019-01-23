---
title: DeviceThreatProtectionLevel Enum-Typ
description: Gerät Bedrohung Schutzebenen für das Gerät Threat Protection-API.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a4c9bbc599d424b91d07339a7a7cdad90b84c262
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411232"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>DeviceThreatProtectionLevel Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Gerät Bedrohung Schutzebenen für das Gerät Threat Protection-API.

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|nicht verfügbar|0|Standardwert. Nicht verwenden.|
|gesichert|1|Gerät veränderte Anforderung: gesichert. Dies ist die sicherste Ebene und steht, die auf dem Gerät keine Viren gefunden wurden.|
|Niedrig|2|Gerät Threat Protection geforderte: niedrig. Niedrig stellt einen Schweregrad der Bedrohung, die an das Gerät oder Gerätedaten minimalem Risiko darstellt.|
|medium|3|Gerät Threat Protection geforderte: Mittel. Mittel stellt einen Schweregrad der Bedrohung, dass Posen Risiko an das Gerät oder Gerätedaten mäßig dar.|
|hohe|4|Gerät Threat Protection geforderte: hoch. Besonders stellt einen Schweregrad der Bedrohung, die an das Gerät oder Gerätedaten erheblich Risiko darstellt.|
|notSet|10|Gerät Threat Protection geforderte: nicht festgelegt. Set darstellt, keine Notwendigkeit für das Gerät besteht zu eine Bedrohung Schutzebene erfüllen.|




