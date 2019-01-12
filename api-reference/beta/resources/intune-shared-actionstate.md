---
title: ActionState Enum-Typ
description: Status der Aktion auf dem Gerät
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 14ec93848deccb7d6bb21331095f9ecf4a881815
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990852"
---
# <a name="actionstate-enum-type"></a>ActionState Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Status der Aktion auf dem Gerät
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|n/v|0|Nicht auf einen gültigen Action Zustand|
|Ausstehende|1|Aktion steht noch aus|
|abgebrochen|2|Aktion wurde abgebrochen.|
|aktive|3|Aktion ist aktiv.|
|done|4|Aktion ohne Fehler abgeschlossen.|
|failed|5|Aktion ist fehlgeschlagen|
|notSupported|6|Aktion wird nicht unterstützt.|





