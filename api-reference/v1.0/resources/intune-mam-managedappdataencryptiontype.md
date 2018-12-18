---
title: ManagedAppDataEncryptionType Enum-Typ
description: Stellt die Ebene an die app-Daten für verwaltete apps verschlüsselt werden
author: tfitzmac
ms.openlocfilehash: 3cbb733eb578ca839e32851d8a6d217f69d6799d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330324"
---
# <a name="managedappdataencryptiontype-enum-type"></a>ManagedAppDataEncryptionType Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt die Ebene an die app-Daten für verwaltete apps verschlüsselt werden
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|useDeviceSettings|0|App-Daten werden verschlüsselt basierend auf die Standardeinstellungen auf dem Gerät.|
|afterDeviceRestart|1|App-Daten werden verschlüsselt, wenn das Gerät neu gestartet wird.|
|whenDeviceLockedExceptOpenFiles|2|App-Daten, die diese Richtlinie zugeordnet werden verschlüsselt, wenn das Gerät, mit Ausnahme von Daten in Dateien gesperrt ist, die geöffnet sind|
|whenDeviceLocked|3|App-Daten, die diese Richtlinie zugeordnet werden verschlüsselt, wenn das Gerät gesperrt ist|



