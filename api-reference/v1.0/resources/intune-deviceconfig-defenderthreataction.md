---
title: DefenderThreatAction Enum-Typ
description: Defender Standardaktion durchführen erkannt Schadsoftware.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 51aa26483ac6b79d48567f7e5950733def31f01e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976646"
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



