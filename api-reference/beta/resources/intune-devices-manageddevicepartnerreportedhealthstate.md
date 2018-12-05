---
title: ManagedDevicePartnerReportedHealthState Enum-Typ
description: Verfügbare Zustände für das Gerät Health-API
ms.openlocfilehash: 3d944eacc2fe94d00fd1b5dd657ba9e936ab78c7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064440"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>ManagedDevicePartnerReportedHealthState Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Verfügbare Zustände für das Gerät Health-API
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Gerät Integritätsstatus ist noch nicht gemeldet.|
|aktiviert|1|Gerät von einem mobilen Threat Defense Partner aktiviert wurde, aber noch nicht Health gemeldet.|
|deaktiviert|2|Gerät wurde von einem mobilen Threat Defense Partner deaktiviert. Die Integrität Gerät ist nicht bekannt.|
|gesichert|3|Gerät gilt als vom mobilen Threat Defense Partner gesichert.|
|lowSeverity|4|Gerät wird vom mobilen Threat Defense Partner geringe Bedrohung angesehen.|
|mediumSeverity|5|Gerät wird vom mobilen Threat Defense Partner mittlere Bedrohung angesehen.|
|highSeverity|6|Gerät wird vom mobilen Threat Defense Partner hohe Bedrohung angesehen.|
|nicht reagiert|7|Gerät gilt vom mobilen Threat Defense Partner nicht reagiert. Die Integrität Gerät ist nicht bekannt.|
|gefährdet|8|Gerät wird durch die Abwehr von Partner gefährdet betrachtet. Dies bedeutet, dass das Gerät verfügt über ein aktives Bedrohung oder Risiko, das vom Endbenutzer auf einfache Weise behoben werden, ist nicht möglich, und der Benutzer sollte ihre IT-Administrator wenden|
|falsch konfiguriert|9|Gerät ist falsch konfiguriert, mit dem Partner Abwehr von berücksichtigt. Dies bedeutet, dass das Gerät fehlt eine erforderliche Profil oder Konfiguration für den Threat Defense Partner ordnungsgemäß funktioniert und ist somit Bedrohung oder Analyse kann nicht für die Durchführung.|




