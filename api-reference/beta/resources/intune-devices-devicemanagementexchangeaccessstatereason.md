---
title: deviceManagementExchangeAccessStateReason-Enumerationstyp
description: Grund für den Zugriffsstatus des Geräteaustauschs.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c788a08e09816683ed575898ee5f36cba241a8bf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175262"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>deviceManagementExchangeAccessStateReason-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Grund für den Zugriffsstatus des Geräteaustauschs.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|Keine|0|Kein aus Exchange ermittelter Zugriffsstatus Grund|
|unknown|1|UnBekannter Zugriffsstatus Grund|
|exchangeGlobalRule|2|Von der globalen Exchange-Regel festgelegter Zugriffsstatus|
|exchangeIndividualRule|3|Von Exchange Individual Rule festgelegter Zugriffsstatus|
|exchangeDeviceRule|4|Von der Exchange-Geräteregel festgelegter Zugriffsstatus|
|exchangeUpgrade|5|Zugriffsstatus aufgrund des Exchange-Upgrades|
|exchangeMailboxPolicy|6|Von Exchange-Postfachrichtlinien festgelegter Zugriffsstatus|
|anderen|7|Von Exchange festgelegter Zugriffsstatus|
|kompatibel|8|Von Compliance Challenge erteilte Zugriffsstatus|
|notCompliant|9|Von Compliance-Herausforderungen gesperrter Zugriffsstatus|
|notEnrolled|10|Von der Verwaltungs Herausforderung gesperrter Zugriffsstatus|
|unknownLocation|12|Zugriffsstatus aufgrund eines unbekannten Standorts|
|mfaRequired|13|Zugriffsstatus aufgrund der MFA-Herausforderung|
|azureADBlockDueToAccessPolicy|14|Von der AAD-Zugriffsrichtlinie gesperrter Zugriffsstatus|
|compromisedPassword|15|Zugriffsstatus, der durch ein kompromittiertes Kennwort widerrufen wurde|
|deviceNotKnownWithManagedApp|16|Von der Herausforderung der verwalteten Anwendung gesperrter Zugriffsstatus|




