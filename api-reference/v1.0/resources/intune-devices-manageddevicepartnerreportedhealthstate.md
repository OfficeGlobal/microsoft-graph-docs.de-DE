---
title: ManagedDevicePartnerReportedHealthState Enum-Typ
description: Verfügbare Zustände für das Gerät Health-API
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9c714c9ed2b070106a37b41712eeb29210d98e60
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841251"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>ManagedDevicePartnerReportedHealthState Enum-Typ

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



