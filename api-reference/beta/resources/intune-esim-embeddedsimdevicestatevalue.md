---
title: embeddedSIMDeviceStateValue-Enumerationstyp
description: Beschreibt die verschiedenen Status für einen eingebetteten SIM-Aktivierungscode.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9bdc3250605de7db7a3778d64b5e743a415de4c0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145423"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>embeddedSIMDeviceStateValue-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Beschreibt die verschiedenen Status für einen eingebetteten SIM-Aktivierungscode.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|notEvaluated|0|Gibt an, dass der eingebettete SIM-Aktivierungscode kostenlos ist und einem Gerät zugewiesen werden kann.|
|failed|1|Gibt an, dass InTune-Dienst dieses Profil nicht an ein Gerät übermitteln konnte.|
|Installieren|2|Gibt an, dass der eingebettete SIM-Aktivierungscode einem Gerät zugewiesen wurde und das Gerät das Token installiert.|
|installiert|3|Gibt an, dass der eingebettete SIM-Aktivierungscode erfolgreich auf dem Zielgerät installiert wurde.|
|Löschen|4|Gibt an, dass InTune-Dienst versucht, das Profil vom Gerät zu löschen.|
|error|5|Gibt an, dass ein Fehler mit diesem Profil vorliegt.|
|deleted|6|Legt fest, dass das Profil vom Gerät gelöscht wird.|
|removedByUser|7|Legt fest, dass das Profil vom Benutzer vom Gerät entfernt wurde.|




