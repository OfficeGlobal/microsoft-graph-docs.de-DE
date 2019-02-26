---
title: managementState-Enumerationstyp
description: Verwaltungsstatus des Geräts in Microsoft InTune
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a53b07f89ee551d3e559a42bbe23c5fba808f20
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174144"
---
# <a name="managementstate-enum-type"></a>managementState-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Verwaltungsstatus des Geräts in Microsoft InTune

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|verwaltete|0|Das Gerät ist unter Verwaltung|
|retirePending|1|Ein Ruhestands Befehl tritt auf dem Gerät auf und wird während der Registrierung von der Verwaltung abgemeldet.|
|retireFailed|2|Fehler beim Ausführen des Befehls auf dem Gerät|
|wipePending|3|Ein Löschbefehl ist auf dem Gerät und während der Registrierung von der Verwaltung|
|wipeFailed|4|Löschbefehl auf dem Gerät fehlgeschlagen|
|fehlerhaft|5|Das Gerät ist fehlerhaft.|
|deletePending|6|Auf dem Gerät tritt ein Löschbefehl auf. |
|retireIssued|7|Für das Gerät wurde ein Ruhestands Befehl ausgegeben.|
|wipeIssued|8|Für das Gerät wurde ein Löschbefehl ausgegeben.|
|wipeCanceled|9|Ein Löschbefehl für dieses Gerät wurde abgebrochen|
|retireCanceled|10|Ein Ruhestands Befehl für dieses Gerät wurde abgebrochen|
|ermittelt|11|Das Gerät wurde ermittelt, aber nicht vollständig registriert.|




