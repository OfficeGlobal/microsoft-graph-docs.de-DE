---
title: DiagnosticDataSubmissionMode Enum-Typ
description: Zulassen Sie das Gerät zum Senden von Diagnose- und Verwendungsanalyse Telemetriedaten wie Watson.
ms.openlocfilehash: b09a4bf334af5981c3ce6dabbab0ac64e2b24887
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019076"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>DiagnosticDataSubmissionMode Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Zulassen Sie das Gerät zum Senden von Diagnose- und Verwendungsanalyse Telemetriedaten wie Watson.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|vom Typ userDefined|0|Ermöglicht es dem Benutzer festgelegt.|
|n/v|1|Keine Telemetriedaten werden von Betriebssystemkomponenten gesendet. Hinweis: Dieser Wert gilt nur für Enterprise und Server-Geräte. Mit dieser Einstellung auf anderen Geräten entspricht dem Festlegen des Werts von 1.|
|grundlegende|2|Grundlegende Telemetriedaten sendet.|
|Erweiterte|3|Sendet erweiterten Telemetriedaten, einschließlich der Verwendung und Einblicke in die Daten.|
|vollständige|4|Sendet vollständige Telemetriedaten einschließlich Diagnosedaten wie Systemstatus.|



