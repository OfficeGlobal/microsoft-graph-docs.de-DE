---
title: windowsDeliveryOptimizationMode-Enumerationstyp
description: Bereitstellungs Optimierungsmodus für die Peer Verteilung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a4b0860e05d20ea480f9c91264033f7a9eb41a0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149168"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Bereitstellungs Optimierungsmodus für die Peer Verteilung

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|userDefined|0|Zulassen, dass der Benutzer festgelegt wird.|
|"HttpOnly"|1|Nur HTTP, kein Peering|
|httpWithPeeringNat|2|Betriebssystemstandard – http-Überblendung mit Peering hinter demselben Netzwerkadressübersetzer|
|httpWithPeeringPrivateGroup|3|HTTP-Überblendung mit Peering über eine private Gruppe hinweg|
|httpWithInternetPeering|4|HTTP-Blended mit Internet-Peering|
|simpleDownload|99|Einfacher Downloadmodus ohne Peering|
|bypassMode|100|Umgehungsmodus. Verwenden Sie keine BereitstellungsOptimierung und verwenden Sie stattdessen BITS.|




