---
title: DiagnosticDataSubmissionMode Enum-Typ
description: Zulassen Sie das Gerät zum Senden von Diagnose- und Verwendungsanalyse Telemetriedaten wie Watson.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b587d6872bcd3610c3b878ae7a672c3e776ea01
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422257"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>DiagnosticDataSubmissionMode Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Zulassen Sie das Gerät zum Senden von Diagnose- und Verwendungsanalyse Telemetriedaten wie Watson.

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|vom Typ userDefined|0|Ermöglicht es dem Benutzer festgelegt.|
|Keine|1|Keine Telemetriedaten werden von Betriebssystemkomponenten gesendet. Hinweis: Dieser Wert gilt nur für Enterprise und Server-Geräte. Mit dieser Einstellung auf anderen Geräten entspricht dem Festlegen des Werts von 1.|
|grundlegende|2|Grundlegende Telemetriedaten sendet.|
|Erweiterte|3|Sendet erweiterten Telemetriedaten, einschließlich der Verwendung und Einblicke in die Daten.|
|vollständige|4|Sendet vollständige Telemetriedaten einschließlich Diagnosedaten wie Systemstatus.|




