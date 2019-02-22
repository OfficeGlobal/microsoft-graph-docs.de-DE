---
title: dmaGuardDeviceEnumerationPolicyType-Enumerationstyp
description: Mögliche Werte des DmaGuardDeviceEnumerationPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 512bf44d25629f4b1c88c2309c464e9d0f33f625
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159710"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a>dmaGuardDeviceEnumerationPolicyType-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Mögliche Werte des DmaGuardDeviceEnumerationPolicy.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Standardwert. Geräte mit inkompatiblen DMA-Treibern werden nur aufgelistet, nachdem der Benutzer den Bildschirm aufgehoben hat.|
|blockAll|1|Geräte mit inkompatiblen DMA-Treibern können nie mehr gestartet und DMA ausführen.|
|allowAll|2|Alle externen DMA-fähigen PCIe-Geräte werden jederzeit aufgelistet.|




