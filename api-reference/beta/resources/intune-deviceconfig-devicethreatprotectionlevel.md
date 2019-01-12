---
title: DeviceThreatProtectionLevel Enum-Typ
description: Gerät Bedrohung Schutzebenen für das Gerät Threat Protection-API.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38d4c17fc9883b23417a4c72ac7cc3c75512865c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948051"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>DeviceThreatProtectionLevel Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Gerät Bedrohung Schutzebenen für das Gerät Threat Protection-API.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|nicht verfügbar|0|Standardwert. Nicht verwenden.|
|gesichert|1|Gerät veränderte Anforderung: gesichert. Dies ist die sicherste Ebene und steht, die auf dem Gerät keine Viren gefunden wurden.|
|Niedrig|2|Gerät Threat Protection geforderte: niedrig. Niedrig stellt einen Schweregrad der Bedrohung, die an das Gerät oder Gerätedaten minimalem Risiko darstellt.|
|medium|3|Gerät Threat Protection geforderte: Mittel. Mittel stellt einen Schweregrad der Bedrohung, dass Posen Risiko an das Gerät oder Gerätedaten mäßig dar.|
|hohe|4|Gerät Threat Protection geforderte: hoch. Besonders stellt einen Schweregrad der Bedrohung, die an das Gerät oder Gerätedaten erheblich Risiko darstellt.|
|notSet|10|Gerät Threat Protection geforderte: nicht festgelegt. Set darstellt, keine Notwendigkeit für das Gerät besteht zu eine Bedrohung Schutzebene erfüllen.|





