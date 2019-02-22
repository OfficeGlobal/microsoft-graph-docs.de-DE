---
title: Eigenschaften automaticupdatemode-Enumerationstyp
description: Mögliche Werte für den automatischen Aktualisierungsmodus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bba7addc5ae3b7942c3e52e1d8989100e27b2831
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156784"
---
# <a name="automaticupdatemode-enum-type"></a>Eigenschaften automaticupdatemode-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Mögliche Werte für den automatischen Aktualisierungsmodus.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|userDefined|0|Benutzerdefiniert, Standardwert, keine Absicht.|
|notifyDownload|1|Benachrichtigung beim Download.|
|autoInstallAtMaintenanceTime|2|Automatische Installation zur Wartungszeit.|
|autoInstallAndRebootAtMaintenanceTime|3|Automatisches Installieren und Neustarten zum Zeitpunkt der Wartung.|
|autoInstallAndRebootAtScheduledTime|4|Automatisches Installieren und Neustarten zum geplanten Zeitpunkt.|
|autoInstallAndRebootWithoutEndUserControl|5|Automatisches Installieren und Neustarten ohne Endbenutzer Steuerelement|
|windowsDefault|6|Zurücksetzen auf Windows-Standardwert.|




