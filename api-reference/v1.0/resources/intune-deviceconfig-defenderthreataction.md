---
title: DefenderThreatAction Enum-Typ
description: Defender Standardaktion durchführen erkannt Schadsoftware.
localization_priority: Normal
ms.openlocfilehash: ed84a16dbac493a3e962e37ba246d8d418782a91
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852822"
---
# <a name="defenderthreataction-enum-type"></a>DefenderThreatAction Enum-Typ

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



