---
title: DeviceRegistrationState Enum-Typ
description: Registrierung Gerätestatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 90f2dc7f8c11940fa01047d8c61f23c8f0389ed8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396756"
---
# <a name="deviceregistrationstate-enum-type"></a>DeviceRegistrationState Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Registrierung Gerätestatus.

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|nicht registriert|0|Das Gerät ist nicht registriert.|
|registriert|2|Das Gerät registriert ist.|
|widerrufen|3|Das Gerät wurde blockiert, gelöscht oder zurückgezogen.|
|keyConflict|4|Das Gerät hat einen Konflikt mit Schlüssel.|
|approvalPending|5|Das Gerät ist ausstehender Genehmigung.|
|certificateReset|6|Das Gerät Zertifikat wurde zurückgesetzt.|
|notRegisteredPendingEnrollment|7|Das Gerät ist nicht registriert und ausstehenden Registrierung.|
|unknown|8|Die Registrierung Gerätestatus ist unbekannt.|




