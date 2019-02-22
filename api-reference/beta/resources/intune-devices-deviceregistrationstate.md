---
title: deviceRegistrationState-Enumerationstyp
description: Status der Geräteregistrierung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f04d8c0fddb966504675e3b4c677dfd0bbabe64c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144625"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Status der Geräteregistrierung.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|notRegistered|0|Das Gerät ist nicht registriert.|
|registriert|2|Das Gerät ist registriert.|
|gesperrt|3|Das Gerät wurde gesperrt, gelöscht oder im Ruhestand.|
|keyConflict|4|Das Gerät hat einen Schlüsselkonflikt.|
|approvalPending|5|Das Gerät steht zur Genehmigung.|
|certificateReset|6|Das Gerätezertifikat wurde zurückgesetzt.|
|notRegisteredPendingEnrollment|7|Das Gerät ist nicht registriert und steht noch aus der Registrierung.|
|unknown|8|Der Geräte Registrierungsstatus ist unbekannt.|




