---
title: windowsDeliveryOptimizationMode-Enumerationstyp
description: Bereitstellungs Optimierungsmodus für die Peer Verteilung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9034c7c90257a7ca622cd203d4ab84387fd2014
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251503"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a>windowsDeliveryOptimizationMode-Enumerationstyp

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



