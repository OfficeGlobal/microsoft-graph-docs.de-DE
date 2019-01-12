---
title: ManagementState Enum-Typ
description: Verwaltungsstatus des Geräts in Microsoft Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7d9d083c56df366b9f896432328d51c295f62190
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961946"
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





