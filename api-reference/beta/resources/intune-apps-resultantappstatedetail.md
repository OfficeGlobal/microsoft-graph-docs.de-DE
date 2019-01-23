---
title: ResultantAppStateDetail Enum-Typ
description: Enum angibt, Weitere Einzelheiten zu warum eine Anwendung für einen bestimmten hat Installationsstatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 34b4d885f9ed2a23669bc2e30c91de40af8d915b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410238"
---
# <a name="resultantappstatedetail-enum-type"></a>ResultantAppStateDetail Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Enum angibt, Weitere Einzelheiten zu warum eine Anwendung für einen bestimmten hat Installationsstatus.

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|noAdditionalDetails|0|Es sind keine weiteren Details verfügbar.|
|seeInstallErrorCode|2000|Anwendung konnte nicht installiert werden. Finden Sie unter Error Code-Eigenschaft für weitere Details.|
|seeUninstallErrorCode|4000|Anwendung konnte nicht deinstalliert werden. Finden Sie unter Error Code-Eigenschaft für weitere Details.|
|pendingReboot|5000|Gerät muss neu gestartet werden, um die Installation der Anwendung abzuschließen.|
|platformNotApplicable|-1006|Anwendung gilt nicht für diese Plattform. (z. B. Android-app Ziel IOS)|
|minimumCpuSpeedNotMet|-1005|CPU-Geschwindigkeit auf das Zielgerät ist kleiner als die minimal konfigurierten.|
|minimumLogicalProcessorCountNotMet|-1004|Anzahl der logischen Prozessoren auf dem Zielgerät ist kleiner als die minimal konfigurierten.|
|minimumPhysicalMemoryNotMet|-1003|Größe des Arbeitsspeichers auf das Zielgerät ist kleiner als die minimal konfigurierten.|
|minimumOsVersionNotMet|-1002|Version des Betriebssystems auf das Zielgerät ist kleiner als die minimal konfigurierten.|
|minimumDiskSpaceNotMet|-1001|Verfügbarer Speicherplatz auf dem Zielgerät ist kleiner als die minimal konfigurierten.|
|processorArchitectureNotApplicable|-1000|Gerätearchitektur (z. B. X86/amd64) gilt nicht für die Anwendung.|




