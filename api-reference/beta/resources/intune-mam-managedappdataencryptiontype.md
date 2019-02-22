---
title: managedAppDataEncryptionType-Enumerationstyp
description: Stellt die Ebene dar, auf die APP-Daten für verwaltete apps verschlüsselt werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47396f32ed23234c5fe758a29b6e97ee3602234f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159080"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt die Ebene dar, auf die APP-Daten für verwaltete apps verschlüsselt werden.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|useDeviceSettings|0|App-Daten werden basierend auf den Standardeinstellungen auf dem Gerät verschlüsselt.|
|afterDeviceRestart|1|App-Daten werden beim Neustart des Geräts verschlüsselt.|
|whenDeviceLockedExceptOpenFiles|2|App-Daten, die dieser Richtlinie zugeordnet sind, werden verschlüsselt, wenn das Gerät gesperrt ist, mit Ausnahme von Daten in geöffneten Dateien|
|whenDeviceLocked|3|App-Daten, die dieser Richtlinie zugeordnet sind, werden verschlüsselt, wenn das Gerät gesperrt ist.|




