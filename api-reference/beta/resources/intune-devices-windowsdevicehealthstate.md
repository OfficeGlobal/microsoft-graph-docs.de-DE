---
title: windowsDeviceHealthState-Enumerationstyp
description: Schutzstatus des Computer Endpunkts
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb335cd39e6cbcd00f754faae8f7784001c424b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156168"
---
# <a name="windowsdevicehealthstate-enum-type"></a>windowsDeviceHealthState-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Schutzstatus des Computer Endpunkts

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|clean|0|Der Computer ist sauber, und es ist keine Aktion erforderlich.|
|fullScanPending|1|Der Computer ist in ausstehender vollständiger Scanstatus|
|rebootPending|2|Der Computer befindet sich im ausstehenden Neustartstatus|
|manualStepsPending|4|Der Computer befindet sich in ausstehenden manuellen Schritten Status|
|offlineScanPending|8|Der Computer befindet sich im ausstehenden Offline Scanstatus|
|critical|16|Der Computer befindet sich im Status "kritisch"|




