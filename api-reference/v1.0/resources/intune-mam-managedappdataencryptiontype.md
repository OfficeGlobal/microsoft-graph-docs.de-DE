---
title: managedAppDataEncryptionType-Enumerationstyp
description: Stellt die Ebene dar, auf die APP-Daten für verwaltete apps verschlüsselt werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 774312d5f19b223fd33e2c156610f516ae7f48a3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256770"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType-Enumerationstyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt die Ebene dar, auf die APP-Daten für verwaltete apps verschlüsselt werden.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|useDeviceSettings|0|App-Daten werden basierend auf den Standardeinstellungen auf dem Gerät verschlüsselt.|
|afterDeviceRestart|1|App-Daten werden beim Neustart des Geräts verschlüsselt.|
|whenDeviceLockedExceptOpenFiles|2|App-Daten, die dieser Richtlinie zugeordnet sind, werden verschlüsselt, wenn das Gerät gesperrt ist, mit Ausnahme von Daten in geöffneten Dateien|
|whenDeviceLocked|3|App-Daten, die dieser Richtlinie zugeordnet sind, werden verschlüsselt, wenn das Gerät gesperrt ist.|



