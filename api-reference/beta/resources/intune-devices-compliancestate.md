---
title: complianceState-Enumerationstyp
description: Konformitätsstatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29357c5248aea78ffca8af464ecf4c3af17bdbc3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172926"
---
# <a name="compliancestate-enum-type"></a>complianceState-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Konformitätsstatus.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Unbekannt.|
|kompatibel|1|Kompatibel.|
|konform|2|Das Gerät ist nicht kompatibel und wird von Unternehmensressourcen blockiert.|
|Konflikt|3|Konflikt mit anderen Regeln.|
|error|4|Fehler|
|inGracePeriod|254|Das Gerät ist nicht kompatibel, hat jedoch weiterhin Zugriff auf Unternehmensressourcen.|
|configManager|255|Verwaltet von config Manager|




