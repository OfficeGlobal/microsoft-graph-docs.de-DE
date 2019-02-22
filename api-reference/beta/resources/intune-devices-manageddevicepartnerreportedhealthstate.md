---
title: managedDevicePartnerReportedHealthState-Enumerationstyp
description: Verfügbare Integritätsstatus für die Geräte Integritäts-API
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60a3071094e2667b896401c6df29977f9923884c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143771"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>managedDevicePartnerReportedHealthState-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Verfügbare Integritätsstatus für die Geräte Integritäts-API

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Der Geräte Integritätsstatus wurde noch nicht gemeldet.|
|aktiviert|1|Das Gerät wurde von einem mobilen Bedrohungsabwehr Partner aktiviert, hat aber noch keinen Status gemeldet.|
|deaktiviert|2|Das Gerät wurde von einem mobilen Bedrohungsabwehr Partner deaktiviert. Der Gerätestatus ist unbekannt.|
|gesichert|3|Gerät gilt als durch den mobilen Threat Defense-Partner gesichert.|
|lowSeverity|4|Gerät gilt als geringe Bedrohung durch den mobilen Threat Defense-Partner.|
|mediumSeverity|5|Gerät gilt als mittlere Bedrohung durch den mobilen Threat Defense-Partner.|
|highSeverity|6|Gerät gilt als hohe Bedrohung durch den mobilen Threat Defense-Partner.|
|reagiert|7|Gerät gilt nicht für den mobilen Threat Defense-Partner. Der Gerätestatus ist unbekannt.|
|gefährdet|8|Das Gerät wird vom BedrohungsAbwehr Partner als kompromittiert betrachtet. Dies hat zur Folge, dass das Gerät eine aktive Bedrohung oder ein Risiko hat, das vom Endbenutzer nicht einfach wiederhergestellt werden kann und der Benutzer sich an seinen IT-Administrator wenden sollte.|
|falsch konfigurierter|9|Gerät wird als falsch konfiguriert mit dem Threat Defense Partner betrachtet. Das bedeutet, dass dem Gerät ein erforderliches Profil oder eine Konfiguration fehlt, damit der Threat Defense-Partner ordnungsgemäß funktioniert und daher eine Bedrohungs-oder Risikoanalyse nicht abgeschlossen werden kann.|




