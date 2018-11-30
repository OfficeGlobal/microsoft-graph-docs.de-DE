---
title: ResultantAppStateDetail Enum-Typ
description: Enum angibt, Weitere Einzelheiten zu warum eine Anwendung für einen bestimmten hat Installationsstatus.
ms.openlocfilehash: 6557047249483273abff93bbbd352cba72256755
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062434"
---
# <a name="resultantappstatedetail-enum-type"></a>ResultantAppStateDetail Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Enum angibt, Weitere Einzelheiten zu warum eine Anwendung für einen bestimmten hat Installationsstatus.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
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





