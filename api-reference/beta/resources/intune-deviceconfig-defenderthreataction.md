---
title: defenderThreatAction-Enumerationstyp
description: Die Standardaktion des Verteidigers für erkannte Schadsoftware.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4849f369aa5dd04a68599050aa097b2ac63f5ef1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154782"
---
# <a name="defenderthreataction-enum-type"></a>defenderThreatAction-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Standardaktion des Verteidigers für erkannte Schadsoftware.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Anwenden einer Aktion basierend auf der Updatedefinition.|
|clean|1|BeReinigen Sie die erkannte Bedrohung.|
|Quarantäne|2|Isolieren Sie die erkannte Bedrohung.|
|remove|3|Entfernen Sie die erkannte Bedrohung.|
|zulassen|4|Die erkannte Bedrohung zulassen.|
|userDefined|5|Der Benutzer kann die Aktion bestimmen, die mit der erkannten Bedrohung ausgeführt werden soll.|
|Block|6|Die erkannte Bedrohung blockieren.|




