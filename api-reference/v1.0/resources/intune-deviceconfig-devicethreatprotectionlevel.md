---
title: DeviceThreatProtectionLevel Enum-Typ
description: Gerät Bedrohung Schutzebenen für das Gerät Threat Protection-API.
author: tfitzmac
ms.openlocfilehash: 755fd861196839ec261dd18f458b88aa97cf0191
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356007"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>DeviceThreatProtectionLevel Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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



