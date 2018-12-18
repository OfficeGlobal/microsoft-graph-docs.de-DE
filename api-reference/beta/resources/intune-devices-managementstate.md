---
title: ManagementState Enum-Typ
description: Verwaltungsstatus des Geräts in Microsoft Intune.
author: tfitzmac
ms.openlocfilehash: 530c1fec4effeb83f6efb635cd44995d904dbdcf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361061"
---
# <a name="managementstate-enum-type"></a>ManagementState Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Verwaltungsstatus des Geräts in Microsoft Intune.
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|verwaltete|0|Das Gerät ist, klicken Sie unter Verwaltung|
|retirePending|1|Ein Außerkraftsetzungsrichtlinie Befehl ist nicht mehr auftritt, auf dem Gerät und gerade unenrolling aus der Verwaltung|
|retireFailed|2|Stilllegung der Befehl auf dem Gerät fehlgeschlagen|
|wipePending|3|Ein Remotegerätzurücksetzung Befehl ist nicht mehr auftritt, auf dem Gerät und gerade unenrolling aus der Verwaltung|
|wipeFailed|4|Wischen Sie Fehler auf dem Gerät|
|fehlerhaft|5|Das Gerät ist fehlerhaft.|
|deletePending|6|Ein Löschbefehl ist nicht mehr auftritt, auf dem Gerät |
|retireIssued|7|Ein Befehl Außerkraftsetzungsrichtlinie wurde für das Gerät ausgestellt.|
|wipeIssued|8|Ein Befehl Remotegerätzurücksetzung wurde für das Gerät ausgestellt.|
|wipeCanceled|9|Ein Befehl Remotegerätzurücksetzung für dieses Gerät wurde abgebrochen|
|retireCanceled|10|Ein Befehl Außerkraftsetzungsrichtlinie für dieses Gerät wurde abgebrochen|
|ermittelt|11|Das Gerät wird erkannt, aber nicht vollständig registriert.|





