---
title: deviceThreatProtectionLevel-Enumerationstyp
description: Geräte Bedrohungsschutz-Ebenen für die Geräte BedrohungsSchutz-API.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1af0231e15cfa815d3fd2e154adf180f3e0c0c43
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253295"
---
# <a name="devicethreatprotectionlevel-enum-type"></a>deviceThreatProtectionLevel-Enumerationstyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Geräte Bedrohungsschutz-Ebenen für die Geräte BedrohungsSchutz-API.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|verfügbar|0|Standardwert. Nicht verwenden.|
|gesichert|1|Anforderung der Geräte BedrohungsStufe: gesichert. Dies ist die sicherste Stufe und stellt dar, dass auf dem Gerät keine Bedrohungen gefunden wurden.|
|mit niedriger|2|Anforderung an die Geräte Bedrohungsstufe: niedrig. Low stellt einen Schweregrad der Bedrohung dar, der ein minimales Risiko für die Geräte-oder Gerätedaten darstellt.|
|medium|3|Anforderung der Geräte BedrohungsSchutz Stufe: Mittel. Medium stellt einen Schweregrad der Bedrohung dar, der für die Geräte-oder Gerätedaten ein moderates Risiko darstellt.|
|hohe|4|Anforderung an Geräte BedrohungsSchutz: hoch. High stellt einen Schweregrad der Bedrohung dar, der für die Geräte-oder Gerätedaten ein hohes Risiko birgt.|
|notSet|10|Anforderung der Geräte BedrohungsSchutz Ebene: nicht festgelegt. Nicht festgelegt stellt dar, dass das Gerät keine BedrohungsSchutz Ebene erfüllen muss.|



