---
title: ManagementState Enum-Typ
description: Verwaltungsstatus des Geräts in Microsoft Intune.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c439cf0ff830f471d2050eee81c91c6539e66d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844653"
---
# <a name="managementstate-enum-type"></a>ManagementState Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Verwaltungsstatus des Geräts in Microsoft Intune.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
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





