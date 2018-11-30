---
title: DefenderThreatAction Enum-Typ
description: Defender Standardaktion durchführen erkannt Schadsoftware.
ms.openlocfilehash: d6a4ccbc9725c230f6abc7bd9ee1e38a30d5d133
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058157"
---
# <a name="defenderthreataction-enum-type"></a>DefenderThreatAction Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Defender Standardaktion durchführen erkannt Schadsoftware.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Wenden Sie Aktion basierend auf der Definition Update an.|
|clean|1|Bereinigen der erkannten Bedrohung.|
|Quarantäne|2|Isolieren Sie erkannte Bedrohung.|
|remove|3|Erkannte Bedrohung zu entfernen.|
|zulassen|4|Zulassen der erkannten Bedrohung.|
|vom Typ userDefined|5|Ermöglicht es dem Benutzer die erkannten Bedrohung auszuführende Aktion zu bestimmen.|
|Blockieren|6|Blockieren der erkannten Bedrohung.|





