---
title: ManagedAppDataEncryptionType Enum-Typ
description: Stellt die Ebene an die app-Daten für verwaltete apps verschlüsselt werden
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4417d488a1590f8d8e9c40e13118e6ef0dc044d1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944432"
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





