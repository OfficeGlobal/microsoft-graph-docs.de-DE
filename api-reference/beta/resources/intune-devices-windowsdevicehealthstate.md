---
title: WindowsDeviceHealthState Enum-Typ
description: Endpoint Protection-Computerstatus
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2d971de9b20780bb51a19c3417384a0ca0563452
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416349"
---
# <a name="windowsdevicehealthstate-enum-type"></a>WindowsDeviceHealthState Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Endpoint Protection-Computerstatus

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|clean|0|Computer fehlerfrei ist und keine Aktion erforderlich ist|
|fullScanPending|1|Computer befindet sich in ausstehen und vollständigen scan|
|rebootPending|2|Computer befindet sich in Ausstehender Neustart Zustand|
|manualStepsPending|4|Computer befindet sich in ausstehen und manuelle Schritte|
|offlineScanPending|8|Computer befindet sich in offline Scan ausstehen|
|critical|16|Computer befindet sich im kritischen Fehlerzustand|




