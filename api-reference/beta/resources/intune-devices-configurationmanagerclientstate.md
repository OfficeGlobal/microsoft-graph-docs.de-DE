---
title: ConfigurationManagerClientState Enum-Typ
description: Konfigurations-Manager-Clientzustand
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 82f4b677001346f9bd32c1bc54bed6e7fbac253d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425785"
---
# <a name="configurationmanagerclientstate-enum-type"></a>ConfigurationManagerClientState Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Konfigurations-Manager-Clientzustand

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Konfigurations-Manager-Agent ist älter als 1806 oder nicht installiert oder dieses Gerät mehr als 30 Tage lang nicht in Intune eingecheckt wurde.|
|installiert|1|Der Konfigurations-Manager-Agent ist installiert, aber möglicherweise nicht angezeigt werden Sie in der Configuration Manager-Konsole noch. Warten Sie einige Stunden für die Aktualisierung.|
|fehlerfrei|7|Dieses Gerät konnte sich mit den Konfigurations-Manager-Dienst erfolgreich zu überprüfen.|
|installFailed|8|Der Konfigurations-Manager-Agent konnte nicht installiert werden.|
|updateFailed|11|Fehler beim Aktualisieren von Version X y Version der Konfigurations-Manager-Agent. |
|communicationError|19|Der Konfigurations-Manager-Agent in der Vergangenheit den Konfigurations-Manager-Dienst erreichen konnte jedoch kann jetzt nicht mehr. |




