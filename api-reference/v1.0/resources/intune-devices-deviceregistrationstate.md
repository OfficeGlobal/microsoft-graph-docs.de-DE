---
title: deviceRegistrationState-Enumerationstyp
description: Status der Geräteregistrierung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b3bee7ab56f07dd6f27c20c771329ba84edbb19
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264134"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState-Enumerationstyp

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



