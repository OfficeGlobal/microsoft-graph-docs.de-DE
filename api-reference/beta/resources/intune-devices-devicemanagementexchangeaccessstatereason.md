---
title: DeviceManagementExchangeAccessStateReason Enum-Typ
description: Grund der Gerätestatus Exchange-Zugriff.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7a076239e49c59cb95cd1c1f644bc9a2f1f906e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395860"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>DeviceManagementExchangeAccessStateReason Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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




