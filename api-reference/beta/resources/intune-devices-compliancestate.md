---
title: ComplianceState Enum-Typ
description: Compliance-Zustand.
ms.openlocfilehash: c49c0ecc2511f612e743fb5d86a53d150d3fbf45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064425"
---
# <a name="compliancestate-enum-type"></a>ComplianceState Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Compliance-Zustand.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Unbekannt.|
|kompatible|1|Kompatibel.|
|nicht konformer|2|Gerät ist nicht kompatibel und wird von Unternehmensressourcen blockiert.|
|Konflikt|3|Konflikt mit anderen Regeln.|
|error|4|Fehler|
|inGracePeriod|254|Gerät nicht kompatibel ist, aber dennoch hat Zugriff auf Unternehmensressourcen|
|configManager|255|Vom Konfigurations-Manager verwaltet|





