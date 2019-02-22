---
title: firewallPacketQueueingMethodType-Enumerationstyp
description: Mögliche Werte für firewallPacketQueueingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e1b8543df5fa2a50cfdfa56c7cb2d96199ba44e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172205"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>firewallPacketQueueingMethodType-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Mögliche Werte für firewallPacketQueueingMethod

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Kein von InTune konfigurierter Wert, außer Kraft setzen des Standardwerts des Benutzer konfigurierten Geräts|
|deaktiviert|1|Deaktivieren von Paketwarteschlangen|
|queueInbound|2|Eingehende verschlüsselte Pakete in der Warteschlange|
|queueOutbound|3|Entschlüsselte ausgehende Pakete für die Weiterleitung in der Warteschlange|
|queueBoth|4|Warteschlange für ein-und ausgehende Pakete|




