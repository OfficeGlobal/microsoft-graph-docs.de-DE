---
title: DmaGuardDeviceEnumerationPolicyType Enum-Typ
description: Mögliche Werte für die DmaGuardDeviceEnumerationPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5baa0cfd5c80f954036e10f0e4d04d2b83e57f2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430130"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a>DmaGuardDeviceEnumerationPolicyType Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Mögliche Werte für die DmaGuardDeviceEnumerationPolicy.

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Standardwert. Nachdem der Benutzer auf den Bildschirm entsperrt, werden nur Geräte mit DMA Neuzuordnen Treiber kompatibel aufgelistet.|
|blockAll|1|Geräte mit DMA Neuzuordnen inkompatiblen Treiber die nie zum Starten und Ausführen von DMA jederzeit zulässig.|
|allowAll|2|Alle externe DMA PCIe Geräten werden zu einem beliebigen Zeitpunkt aufgelistet werden.|




