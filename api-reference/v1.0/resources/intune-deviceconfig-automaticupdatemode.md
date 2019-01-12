---
title: AutomaticUpdateMode Enum-Typ
description: Mögliche Werte für den Modus für automatische Updates.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a31c50b5d16f4b9be8db4f95f2bbd9bd0ca123e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987860"
---
# <a name="automaticupdatemode-enum-type"></a>AutomaticUpdateMode Enum-Typ

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



