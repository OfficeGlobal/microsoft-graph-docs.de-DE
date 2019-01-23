---
title: ManagementState Enum-Typ
description: Verwaltungsstatus des Geräts in Microsoft Intune.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8d0801949125f3b0cceb865ac1f8546195112e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420017"
---
# <a name="managementstate-enum-type"></a>ManagementState Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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




