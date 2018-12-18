---
title: DeviceManagementExchangeAccessStateReason Enum-Typ
description: Grund der Gerätestatus Exchange-Zugriff.
author: tfitzmac
ms.openlocfilehash: d51e9656c841a86d282eb1b5654da042f91866fd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323443"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>DeviceManagementExchangeAccessStateReason Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Grund der Gerätestatus Exchange-Zugriff.
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|Keine|0|Kein Zugriff Zustand Grund ermittelt aus Exchange|
|unknown|1|Unbekannte Access Zustand Grund|
|exchangeGlobalRule|2|Access-Zustand durch Exchange globale Regel bestimmt|
|exchangeIndividualRule|3|Access-Zustand durch Exchange einzelne Regel bestimmt|
|exchangeDeviceRule|4|Access-Zustand von Exchange-Regel bestimmt|
|exchangeUpgrade|5|Access-Zustand aufgrund von Exchange-upgrade|
|exchangeMailboxPolicy|6|Access-Zustand von Exchange-Postfachrichtlinie bestimmt|
|andere|7|Access-Zustand durch Exchange bestimmt|
|kompatible|8|Greifen Sie Zustand gewährt zu, indem Sie Compliance-Herausforderung|
|notCompliant|9|Access-Status von Compliance-Herausforderung gesperrt|
|notEnrolled|10|Access-Status von Herausforderung Management gesperrt|
|unknownLocation|12|Access-Zustand aufgrund von unbekannten Speicherort|
|mfaRequired|13|Access-Zustand aufgrund mehrstufiger Authentifizierung das Herausforderung|
|azureADBlockDueToAccessPolicy|14|Access-Status von AAD Zugriffsrichtlinie gesperrt|
|compromisedPassword|15|Access-Zustand durch Kennwort offengelegt gesperrt|
|deviceNotKnownWithManagedApp|16|Access-Status von verwalteten Anwendung Herausforderung gesperrt|



