---
title: WindowsDeviceHealthState Enum-Typ
description: Endpoint Protection-Computerstatus
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 628450b33a219e8408d5c5887c6902b78ae02bd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923943"
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





