---
title: resultantAppStateDetail-Enumerationstyp
description: Enum, der zusätzliche Details dazu angibt, warum eine Anwendung einen bestimmten Installationsstatus aufweist.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d6b7e6a665229d02033cd1c0c25469a83dfc37d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167214"
---
# <a name="resultantappstatedetail-enum-type"></a>resultantAppStateDetail-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enum, der zusätzliche Details dazu angibt, warum eine Anwendung einen bestimmten Installationsstatus aufweist.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|noAdditionalDetails|0|Es sind keine weiteren Details verfügbar.|
|seeInstallErrorCode|2000|Die Anwendung konnte nicht installiert werden. Weitere Informationen finden Sie unter Fehlercode-Eigenschaft.|
|seeUninstallErrorCode|4000|Anwendung konnte nicht deinstalliert werden. Weitere Informationen finden Sie unter Fehlercode-Eigenschaft.|
|pendingReboot|5000|Das Gerät muss neu gestartet werden, um die Installation der Anwendung abzuschließen.|
|platformNotApplicable|-1006|Anwendung gilt nicht für diese Plattform. (beispielsweise Android-App für IOS)|
|minimumCpuSpeedNotMet|-1005|Die CPU-Geschwindigkeit auf dem Zielgerät ist kleiner als das konfigurierte Minimum.|
|minimumLogicalProcessorCountNotMet|-1004|Die Anzahl der logischen Prozessoren auf dem Zielgerät ist kleiner als das konfigurierte Minimum.|
|minimumPhysicalMemoryNotMet|-1003|Der RAM-Speicher auf dem Zielgerät ist kleiner als der konfigurierte Mindestwert.|
|minimumOsVersionNotMet|-1002|Die Betriebssystemversion auf dem Zielgerät ist kleiner als das konfigurierte Minimum.|
|minimumDiskSpaceNotMet|-1001|Der verfügbare Speicherplatz auf dem Zielgerät ist kleiner als der konfigurierte Minimalwert.|
|processorArchitectureNotApplicable|-1000|Gerätearchitekturen (beispielsweise x86/amd64) gelten nicht für die Anwendung.|




