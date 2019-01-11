---
title: WindowsDeviceHealthState Enum-Typ
description: Endpoint Protection-Computerstatus
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 91869502d0d61c25c6eb8dd67ba4e8e32d28fbb2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885925"
---
# <a name="windowsdevicehealthstate-enum-type"></a>WindowsDeviceHealthState Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Endpoint Protection-Computerstatus
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|clean|0|Computer fehlerfrei ist und keine Aktion erforderlich ist|
|fullScanPending|1|Computer befindet sich in ausstehen und vollständigen scan|
|rebootPending|2|Computer befindet sich in Ausstehender Neustart Zustand|
|manualStepsPending|4|Computer befindet sich in ausstehen und manuelle Schritte|
|offlineScanPending|8|Computer befindet sich in offline Scan ausstehen|
|critical|16|Computer befindet sich im kritischen Fehlerzustand|





