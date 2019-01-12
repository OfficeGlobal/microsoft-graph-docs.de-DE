---
title: EmailSyncSchedule Enum-Typ
description: Mögliche Werte für e-Mail-Synchronisierungszeitplan.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9dc93bce19262d0b1aad1d1cc8f28ea4db56ce9f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924041"
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





