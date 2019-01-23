---
title: DefenderPotentiallyUnwantedAppAction Enum-Typ
description: Defender Aktion, die auf erkannt potenziell unerwünschte Anwendung (PUA).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2ace0cc29ad284cde63b7e4934fb8cb395f27bbe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422754"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>DefenderPotentiallyUnwantedAppAction Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Defender Aktion, die auf erkannt potenziell unerwünschte Anwendung (PUA).

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|PUA Schutz ist deaktiviert. Defender bietet keinen Schutz vor unerwünschten Applications.|
|Blockieren|1|PUA Schutz ist auf. Erkannte Elemente werden blockiert. Sie werden im Verlauf zusammen mit anderen Bedrohungen angezeigt.|
|Audit|2|Überwachungsmodus aktiviert. Defender unerwünschte Applications erkennen, aber keine Aktionen. Sie können Informationen zu Anwendungen, dass Defender gegen benutzt haben würde durch Suchen des Ereignisse, die in den Ereignisdetails Viewer von Defender erstellt ansehen.|




