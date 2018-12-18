---
title: WindowsDeviceHealthState Enum-Typ
description: Endpoint Protection-Computerstatus
author: tfitzmac
ms.openlocfilehash: b794f8121132e396459f9198c644084690fe95b4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326327"
---
# <a name="windowsdevicehealthstate-enum-type"></a>WindowsDeviceHealthState Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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





