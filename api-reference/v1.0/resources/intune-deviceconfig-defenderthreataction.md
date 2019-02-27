---
title: defenderThreatAction-Enumerationstyp
description: Die Standardaktion des Verteidigers für erkannte Schadsoftware.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d3d48415e55ad246f75ca9b32bd169ee102fc67
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252315"
---
# <a name="defenderthreataction-enum-type"></a>defenderThreatAction-Enumerationstyp

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



