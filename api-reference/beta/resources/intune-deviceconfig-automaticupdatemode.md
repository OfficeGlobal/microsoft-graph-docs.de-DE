---
title: AutomaticUpdateMode Enum-Typ
description: Mögliche Werte für den Modus für automatische Updates.
ms.openlocfilehash: b7eac8337d6c8286e538bbe98b5ecbc13a448628
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063919"
---
# <a name="automaticupdatemode-enum-type"></a>AutomaticUpdateMode Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für den Modus für automatische Updates.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|vom Typ userDefined|0|User-Defined, Standardwert, keine beabsichtigt.|
|notifyDownload|1|Benachrichtigen Sie auf Download.|
|autoInstallAtMaintenanceTime|2|Automatische Installation zur Wartungszeit.|
|autoInstallAndRebootAtMaintenanceTime|3|Automatische Installation und Wartung jederzeit neu starten.|
|autoInstallAndRebootAtScheduledTime|4|Automatische Installation und zum geplanten Zeitpunkt neu starten.|
|autoInstallAndRebootWithoutEndUserControl|5|Automatische Installation und neu starten Sie, ohne Kontrolle durch den Endbenutzer|





