---
title: ManagedAppDataEncryptionType Enum-Typ
description: Stellt die Ebene an die app-Daten für verwaltete apps verschlüsselt werden
ms.openlocfilehash: a642a3efc01f719ca72134f737fe2bdd2596d2b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064082"
---
# <a name="managedappdataencryptiontype-enum-type"></a>ManagedAppDataEncryptionType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt die Ebene an die app-Daten für verwaltete apps verschlüsselt werden
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|useDeviceSettings|0|App-Daten werden verschlüsselt basierend auf die Standardeinstellungen auf dem Gerät.|
|afterDeviceRestart|1|App-Daten werden verschlüsselt, wenn das Gerät neu gestartet wird.|
|whenDeviceLockedExceptOpenFiles|2|App-Daten, die diese Richtlinie zugeordnet werden verschlüsselt, wenn das Gerät, mit Ausnahme von Daten in Dateien gesperrt ist, die geöffnet sind|
|whenDeviceLocked|3|App-Daten, die diese Richtlinie zugeordnet werden verschlüsselt, wenn das Gerät gesperrt ist|





