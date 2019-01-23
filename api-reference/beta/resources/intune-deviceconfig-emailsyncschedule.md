---
title: EmailSyncSchedule Enum-Typ
description: Mögliche Werte für e-Mail-Synchronisierungszeitplan.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8285b9a34e208b86b7c53c38e6aa015fd8c37560
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425183"
---
# <a name="emailsyncschedule-enum-type"></a>EmailSyncSchedule Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Mögliche Werte für e-Mail-Synchronisierungszeitplan.

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|vom Typ userDefined|0|User-Defined, Standardwert, keine beabsichtigt.|
|asMessagesArrive|1|Synchronisieren Sie wie Nachrichten eingehen.|
|Manuell|2|Manuell synchronisieren.|
|fifteenMinutes|3|Synchronisieren Sie alle 15 Minuten.|
|thirtyMinutes|4|Sync alle 30 Minuten.|
|sixtyMinutes|5|Sync alle 60 Minuten.|
|basedOnMyUsage|6|Die Synchronisierung basierend auf meine Verwendung.|




