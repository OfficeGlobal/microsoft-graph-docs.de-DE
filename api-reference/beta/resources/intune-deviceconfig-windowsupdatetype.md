---
title: windowsUpdateType-Enumerationstyp
description: Welche Zweigstellen-Geräte erhalten Ihre Updates von
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17aad82b25982b90ecea348d959e2ed2ec94a483
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169160"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Welche Zweigstellen-Geräte erhalten Ihre Updates von

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|userDefined|0|Zulassen, dass der Benutzer festgelegt wird.|
|all|1|Halbjährlicher Kanal (gezielt). Gerät Ruft alle relevanten Feature-Updates vom halbjährlichen Kanal ab (gezielt).|
|businessReadyOnly|2|Halbjährlicher Kanal. Gerät ruft Feature-Updates vom halbjährlichen Kanal ab.|
|windowsInsiderBuildFast|3|Windows Insider-Erstellung – schnell|
|windowsInsiderBuildSlow|4|Windows Insider Build – langsam|
|windowsInsiderBuildRelease|5|Freigeben von Windows Insider Build|




