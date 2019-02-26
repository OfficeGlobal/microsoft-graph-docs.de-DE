---
title: windowsUpdateType-Enumerationstyp
description: Welche Zweigstellen-Geräte erhalten Ihre Updates von
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f91657cabec59cf1307253d707ba632bf4f99463
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260221"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType-Enumerationstyp

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



