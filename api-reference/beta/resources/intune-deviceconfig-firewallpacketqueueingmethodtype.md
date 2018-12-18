---
title: FirewallPacketQueueingMethodType Enum-Typ
description: Mögliche Werte für firewallPacketQueueingMethod
author: tfitzmac
ms.openlocfilehash: 76d8e886c27e7e0e849a4172dbc763013f4cc5ac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347285"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>FirewallPacketQueueingMethodType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für firewallPacketQueueingMethod
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät|
|deaktiviert|1|Paket Warteschlangen deaktivieren|
|queueInbound|2|Eingehende, verschlüsselte Pakete Warteschlange|
|queueOutbound|3|Warteschlange entschlüsselt ausgehenden Pakete für die Weiterleitung|
|queueBoth|4|Die Warteschlange eingehenden und ausgehenden Pakete|





