---
title: FirewallPacketQueueingMethodType Enum-Typ
description: Mögliche Werte für firewallPacketQueueingMethod
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dc40b93eebc17b1d1abcd9c317da1ffa538512a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425757"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>FirewallPacketQueueingMethodType Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Mögliche Werte für firewallPacketQueueingMethod

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät|
|deaktiviert|1|Paket Warteschlangen deaktivieren|
|queueInbound|2|Eingehende, verschlüsselte Pakete Warteschlange|
|queueOutbound|3|Warteschlange entschlüsselt ausgehenden Pakete für die Weiterleitung|
|queueBoth|4|Die Warteschlange eingehenden und ausgehenden Pakete|




