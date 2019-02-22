---
title: defenderCloudBlockLevelType-Enumerationstyp
description: Mögliche Werte der Cloud-Blockebene
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbf442a11335602c510a210d7bd805b2a76eb7df
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156924"
---
# <a name="defendercloudblockleveltype-enum-type"></a>defenderCloudBlockLevelType-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Mögliche Werte der Cloud-Blockebene

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|notConfigured|0|Standardwert, verwendet die standardmäßige Windows Defender-Antivirus-Blockierungs Ebene und bietet eine starke Erkennung, ohne das Risiko der Erkennung legitimer Dateien zu erhöhen|
|hohe|1|High gilt als starke Erkennungsstufe.|
|highPlus|2|High + verwendet den hohen Level und wendet zusätzliche Schutzmaßnahmen an.|
|zeroTolerance|3|Null Toleranz blockiert alle unbekannten ausführbaren Dateien|




