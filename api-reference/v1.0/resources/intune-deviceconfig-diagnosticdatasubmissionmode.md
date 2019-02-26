---
title: diagnosticDataSubmissionMode-Enumerationstyp
description: Das Gerät kann Diagnose-und Verwendungs Telemetrie-Daten wie Watson senden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c0707b97e60da406210d6a091ed0dd4efaa2299
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251034"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a>diagnosticDataSubmissionMode-Enumerationstyp

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



