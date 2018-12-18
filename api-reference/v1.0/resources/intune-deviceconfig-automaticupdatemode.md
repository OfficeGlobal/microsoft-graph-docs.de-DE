---
title: AutomaticUpdateMode Enum-Typ
description: Mögliche Werte für den Modus für automatische Updates.
author: tfitzmac
ms.openlocfilehash: 01e71e51a47a06aff12dd82e132d7eb468f26229
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346991"
---
# <a name="automaticupdatemode-enum-type"></a>AutomaticUpdateMode Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für den Modus für automatische Updates.
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|vom Typ userDefined|0|User-Defined, Standardwert, keine beabsichtigt.|
|notifyDownload|1|Benachrichtigen Sie auf Download.|
|autoInstallAtMaintenanceTime|2|Automatische Installation zur Wartungszeit.|
|autoInstallAndRebootAtMaintenanceTime|3|Automatische Installation und Wartung jederzeit neu starten.|
|autoInstallAndRebootAtScheduledTime|4|Automatische Installation und zum geplanten Zeitpunkt neu starten.|
|autoInstallAndRebootWithoutEndUserControl|5|Automatische Installation und neu starten Sie, ohne Kontrolle durch den Endbenutzer|



