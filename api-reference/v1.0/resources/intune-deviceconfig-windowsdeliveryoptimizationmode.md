---
title: WindowsDeliveryOptimizationMode Enum-Typ
description: Übermittlung Optimierung Modus für Peer-Verteilung
author: tfitzmac
ms.openlocfilehash: ae61d7dde5fc02ff329eaf9cc970ee7078c3a254
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360158"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>WindowsDeliveryOptimizationMode Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Übermittlung Optimierung Modus für Peer-Verteilung
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|vom Typ userDefined|0|Ermöglicht es dem Benutzer festgelegt.|
|httpOnly|1|Nur HTTP keine peering|
|httpWithPeeringNat|2|OS Standard – gemischt Http mit hinter den gleichen Network Address Translation peering|
|httpWithPeeringPrivateGroup|3|HTTP mit über eine private Gruppe peering gemischt|
|httpWithInternetPeering|4|HTTP mit Internet peering gemischt|
|simpleDownload|99|Einfacher Downloadmodus mit keine peering|
|bypassMode|100|Umgehen Sie Modus. Keine verwenden Sie Übermittlung Optimierung und verwenden Sie stattdessen BITS|



