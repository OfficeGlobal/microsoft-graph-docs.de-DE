---
title: ActionState Enum-Typ
description: Status der Aktion auf dem Gerät
author: tfitzmac
ms.openlocfilehash: 1f36c3a6709ade5860ff24cc8d10c2cb0294a471
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315106"
---
# <a name="actionstate-enum-type"></a>ActionState Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Status der Aktion auf dem Gerät
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|Keine|0|Nicht auf einen gültigen Action Zustand|
|Ausstehende|1|Aktion steht noch aus|
|abgebrochen|2|Aktion wurde abgebrochen.|
|aktive|3|Aktion ist aktiv.|
|done|4|Aktion ohne Fehler abgeschlossen.|
|failed|5|Aktion ist fehlgeschlagen|
|notSupported|6|Aktion wird nicht unterstützt.|





