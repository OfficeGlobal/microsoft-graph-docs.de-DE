---
title: defenderCloudBlockLevelType-Enumerationstyp
description: Mögliche Werte der Cloud-Blockebene
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de81e42827f7c153fc81e7fc19d85e54cb780bfa
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258835"
---
# <a name="defendercloudblockleveltype-enum-type"></a>defenderCloudBlockLevelType-Enumerationstyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Mögliche Werte der Cloud-Blockebene

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|notConfigured|0|Standardwert, verwendet die standardmäßige Windows Defender-Antivirus-Blockierungs Ebene und bietet eine starke Erkennung, ohne das Risiko der Erkennung legitimer Dateien zu erhöhen|
|hohe|1|High gilt als starke Erkennungsstufe.|
|highPlus|2|High + verwendet den hohen Level und wendet zusätzliche Schutzmaßnahmen an.|
|zeroTolerance|3|Null Toleranz blockiert alle unbekannten ausführbaren Dateien|



