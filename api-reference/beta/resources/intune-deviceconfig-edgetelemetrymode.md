---
title: edgeTelemetryMode-Enumerationstyp
description: Art der durchsuchten Daten, die an Microsoft 365 Analytics gesendet werden
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b48840debffcc7aedf1454d9cee11b6c0ab9edc1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172471"
---
# <a name="edgetelemetrymode-enum-type"></a>edgeTelemetryMode-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Art der durchsuchten Daten, die an Microsoft 365 Analytics gesendet werden

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|notConfigured|0|Standard – keine Telemetrie-Daten erfasst oder gesendet|
|Intranet|1|Nur Senden des Intranet-Verlaufs zulassen: nur Senden von Browserverlaufsdaten für Intranet-Websites|
|internet|2|Nur Senden des Internet Verlaufs zulassen: nur Browserverlaufsdaten für Internetwebsites senden|
|intranetAndInternet|3|Senden von Intranet-und Internetprotokollen: Senden von Browserverlaufsdaten für Intranet-und Internetwebsites|




