---
title: DefenderPotentiallyUnwantedAppAction Enum-Typ
description: Defender Aktion, die auf erkannt potenziell unerwünschte Anwendung (PUA).
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 96a3dd70ae0f56f2d0d5a9d6c4f87846e10bba45
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938559"
---
# <a name="defenderpotentiallyunwantedappaction-enum-type"></a>DefenderPotentiallyUnwantedAppAction Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Defender Aktion, die auf erkannt potenziell unerwünschte Anwendung (PUA).
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|PUA Schutz ist deaktiviert. Defender bietet keinen Schutz vor unerwünschten Applications.|
|Blockieren|1|PUA Schutz ist auf. Erkannte Elemente werden blockiert. Sie werden im Verlauf zusammen mit anderen Bedrohungen angezeigt.|
|Audit|2|Überwachungsmodus aktiviert. Defender unerwünschte Applications erkennen, aber keine Aktionen. Sie können Informationen zu Anwendungen, dass Defender gegen benutzt haben würde durch Suchen des Ereignisse, die in den Ereignisdetails Viewer von Defender erstellt ansehen.|





