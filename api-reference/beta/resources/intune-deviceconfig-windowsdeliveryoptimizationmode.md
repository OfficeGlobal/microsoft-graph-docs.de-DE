---
title: WindowsDeliveryOptimizationMode Enum-Typ
description: Übermittlung Optimierung Modus für Peer-Verteilung
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e62416328e596737c36d920d6877773c905680c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807721"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>WindowsDeliveryOptimizationMode Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Übermittlung Optimierung Modus für Peer-Verteilung
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|vom Typ userDefined|0|Ermöglicht es dem Benutzer festgelegt.|
|httpOnly|1|Nur HTTP keine peering|
|httpWithPeeringNat|2|OS Standard – gemischt Http mit hinter den gleichen Network Address Translation peering|
|httpWithPeeringPrivateGroup|3|HTTP mit über eine private Gruppe peering gemischt|
|httpWithInternetPeering|4|HTTP mit Internet peering gemischt|
|simpleDownload|99|Einfacher Downloadmodus mit keine peering|
|bypassMode|100|Umgehen Sie Modus. Keine verwenden Sie Übermittlung Optimierung und verwenden Sie stattdessen BITS|





