---
title: diagnosticDataSubmissionMode-Enumerationstyp
description: Das Gerät kann Diagnose-und Verwendungs Telemetrie-Daten wie Watson senden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e749d2fc7a1eb191c62fbc9db389887cdd901c27
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175220"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>diagnosticDataSubmissionMode-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Das Gerät kann Diagnose-und Verwendungs Telemetrie-Daten wie Watson senden.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|userDefined|0|Zulassen, dass der Benutzer festgelegt wird.|
|Keine|1|Von Betriebssystemkomponenten werden keine Telemetrie-Daten gesendet. Hinweis: dieser Wert gilt nur für Enterprise-und Server-Geräte. Die Verwendung dieser Einstellung auf anderen Geräten entspricht dem Festlegen des Werts 1.|
|Basic|2|Sendet grundlegende Telemetrie-Daten.|
|Erweiterte|3|Sendet erweiterte Telemetrie-Daten, einschließlich Verwendungs-und einblickdaten.|
|vollständige|4|Sendet vollständige Telemetrie-Daten einschließlich Diagnosedaten wie Systemstatus.|




