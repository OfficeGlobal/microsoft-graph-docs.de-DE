---
title: ManagedDevicePartnerReportedHealthState Enum-Typ
description: Verfügbare Zustände für das Gerät Health-API
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cb5b13ceceab27e1e88a69310a3198159f5e24c1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418827"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>ManagedDevicePartnerReportedHealthState Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Verfügbare Zustände für das Gerät Health-API

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
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




