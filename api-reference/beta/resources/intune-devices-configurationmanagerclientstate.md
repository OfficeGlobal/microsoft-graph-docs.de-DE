---
title: ConfigurationManagerClientState Enum-Typ
description: Konfigurations-Manager-Clientzustand
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fc6f3f2db68273097d70ba9dccc6844b86afa3f6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923887"
---
# <a name="configurationmanagerclientstate-enum-type"></a>ConfigurationManagerClientState Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Konfigurations-Manager-Clientzustand
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Konfigurations-Manager-Agent ist älter als 1806 oder nicht installiert oder dieses Gerät mehr als 30 Tage lang nicht in Intune eingecheckt wurde.|
|installiert|1|Der Konfigurations-Manager-Agent ist installiert, aber möglicherweise nicht angezeigt werden Sie in der Configuration Manager-Konsole noch. Warten Sie einige Stunden für die Aktualisierung.|
|fehlerfrei|7|Dieses Gerät konnte sich mit den Konfigurations-Manager-Dienst erfolgreich zu überprüfen.|
|installFailed|8|Der Konfigurations-Manager-Agent konnte nicht installiert werden.|
|updateFailed|11|Fehler beim Aktualisieren von Version X y Version der Konfigurations-Manager-Agent. |
|communicationError|19|Der Konfigurations-Manager-Agent in der Vergangenheit den Konfigurations-Manager-Dienst erreichen konnte jedoch kann jetzt nicht mehr. |





