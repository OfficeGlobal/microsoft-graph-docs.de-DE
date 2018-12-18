---
title: ComplianceState Enum-Typ
description: Compliance-Zustand.
author: tfitzmac
ms.openlocfilehash: 3045685518f1c7718f9a5f46cd10e0add6fe05b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330275"
---
# <a name="compliancestate-enum-type"></a>ComplianceState Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Compliance-Zustand.
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Unbekannt.|
|kompatible|1|Kompatibel.|
|nicht konformer|2|Gerät ist nicht kompatibel und wird von Unternehmensressourcen blockiert.|
|Konflikt|3|Konflikt mit anderen Regeln.|
|error|4|Fehler|
|inGracePeriod|254|Gerät nicht kompatibel ist, aber dennoch hat Zugriff auf Unternehmensressourcen|
|configManager|255|Vom Konfigurations-Manager verwaltet|



