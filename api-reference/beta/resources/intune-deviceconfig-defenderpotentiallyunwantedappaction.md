---
title: DefenderPotentiallyUnwantedAppAction Enum-Typ
description: Defender Aktion, die auf erkannt potenziell unerwünschte Anwendung (PUA).
ms.openlocfilehash: c786906046d6a35c026da95246016537e4325aab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060201"
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





