---
title: EmailSyncSchedule Enum-Typ
description: Mögliche Werte für e-Mail-Synchronisierungszeitplan.
ms.openlocfilehash: 48c5d433815d5f27d018d97ac479641146754669
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058300"
---
# <a name="emailsyncschedule-enum-type"></a>EmailSyncSchedule Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für e-Mail-Synchronisierungszeitplan.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|vom Typ userDefined|0|User-Defined, Standardwert, keine beabsichtigt.|
|asMessagesArrive|1|Synchronisieren Sie wie Nachrichten eingehen.|
|Manuell|2|Manuell synchronisieren.|
|fifteenMinutes|3|Synchronisieren Sie alle 15 Minuten.|
|thirtyMinutes|4|Sync alle 30 Minuten.|
|sixtyMinutes|5|Sync alle 60 Minuten.|
|basedOnMyUsage|6|Die Synchronisierung basierend auf meine Verwendung.|





