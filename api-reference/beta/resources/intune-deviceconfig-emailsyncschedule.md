---
title: EmailSyncSchedule Enum-Typ
description: Mögliche Werte für e-Mail-Synchronisierungszeitplan.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 178cba9e226b7f20e3fd917145e7bbd06f6c3a1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838395"
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





