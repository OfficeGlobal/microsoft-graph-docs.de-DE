---
title: DiagnosticDataSubmissionMode Enum-Typ
description: Zulassen Sie das Gerät zum Senden von Diagnose- und Verwendungsanalyse Telemetriedaten wie Watson.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a293288c3891f8ecd77d422986e419d2e3d53767
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912946"
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



