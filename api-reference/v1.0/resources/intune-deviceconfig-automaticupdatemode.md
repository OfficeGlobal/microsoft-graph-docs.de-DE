---
title: Eigenschaften automaticupdatemode-Enumerationstyp
description: Mögliche Werte für den automatischen Aktualisierungsmodus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fd45ff85cbab934aa2549f13ee3e6671c65f9ae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251377"
---
# <a name="automaticupdatemode-enum-type"></a>Eigenschaften automaticupdatemode-Enumerationstyp

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



