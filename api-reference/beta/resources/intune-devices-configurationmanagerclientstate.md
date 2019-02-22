---
title: configurationManagerClientState-Enumerationstyp
description: Konfigurations-Manager-Client – Status
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe8474e6886c1312fde4ce3afde3c3fe0185574c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170700"
---
# <a name="configurationmanagerclientstate-enum-type"></a>configurationManagerClientState-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Konfigurations-Manager-Client – Status

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Der Configuration Manager-Agent ist älter als 1806 oder nicht installiert, oder dieses Gerät wurde seit über 30 Tagen nicht in InTune eingecheckt.|
|installiert|1|Der Configuration Manager-Agent ist installiert, wird jedoch möglicherweise noch nicht in der Configuration Manager-Konsole angezeigt. Warten Sie einige Stunden, bis es aktualisiert wird.|
|gesunde|7|Dieses Gerät konnte den Configuration Manager-Dienst erfolgreich einchecken.|
|installFailed|8|Fehler beim Installieren des Configuration Manager-Agents.|
|updateFailed|11|Fehler bei der Aktualisierung von Version x auf Version y des Configuration Manager-Agents. |
|communicationError|19|Der Configuration Manager-Agent konnte den Configuration Manager-Dienst in der Vergangenheit erreichen, ist aber jetzt nicht mehr in der Lage. |




