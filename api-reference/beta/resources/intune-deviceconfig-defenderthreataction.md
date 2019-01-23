---
title: DefenderThreatAction Enum-Typ
description: Defender Standardaktion durchführen erkannt Schadsoftware.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d092d5a23fc006a9accdf9062a27cd79f323d208
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400270"
---
# <a name="defenderthreataction-enum-type"></a>DefenderThreatAction Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Defender Standardaktion durchführen erkannt Schadsoftware.

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Wenden Sie Aktion basierend auf der Definition Update an.|
|clean|1|Bereinigen der erkannten Bedrohung.|
|Quarantäne|2|Isolieren Sie erkannte Bedrohung.|
|remove|3|Erkannte Bedrohung zu entfernen.|
|zulassen|4|Zulassen der erkannten Bedrohung.|
|vom Typ userDefined|5|Ermöglicht es dem Benutzer die erkannten Bedrohung auszuführende Aktion zu bestimmen.|
|Blockieren|6|Blockieren der erkannten Bedrohung.|




