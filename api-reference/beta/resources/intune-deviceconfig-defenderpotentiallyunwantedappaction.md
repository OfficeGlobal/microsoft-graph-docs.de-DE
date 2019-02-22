---
title: defenderPotentiallyUnwantedAppAction-Enumerationstyp
description: Die Aktion des Verteidigers zur Übernahme erkannter potenziell unerwünschter Anwendungen (PUA).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02ac5da63c2787c2b87479a23899c9d2980c54c4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173353"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>defenderPotentiallyUnwantedAppAction-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Aktion des Verteidigers zur Übernahme erkannter potenziell unerwünschter Anwendungen (PUA).

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|PUA-Schutz ist deaktiviert. Defender schützt nicht vor potenziell unerwünschten Anwendungen.|
|Block|1|PUA-Schutz ist eingeschaltet. Erkannte Elemente werden blockiert. Sie werden im Verlauf zusammen mit anderen Bedrohungen angezeigt.|
|Audit|2|Überwachungsmodus. Defender ermittelt potenziell unerwünschte Anwendungen, aber keine Aktionen. Sie können Informationen zu Anwendungen, die Defender ergriffen haben, durchsuchen nach von Defender erstellten Ereignissen in der Ereignisanzeige lesen.|




