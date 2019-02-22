---
title: deviceGuardLocalSystemAuthorityCredentialGuardType-Enumerationstyp
description: Mögliche Werte der Einstellungen für den Anmelde Informationenschutz.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8452f24f0bc5641d9d7ebcfd68c8cd593443554d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167858"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a>deviceGuardLocalSystemAuthorityCredentialGuardType-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Mögliche Werte der Einstellungen für den Anmelde Informationenschutz.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|notConfigured|0|Deaktiviert die Überwachung der Anmeldeinformationen, wenn Sie zuvor ohne UEFI-Sperre konfiguriert wurden.|
|enableWithUEFILock|1|Aktiviert den Schutz von Anmeldeinformationen mit UEFI-Sperre.|
|enableWithoutUEFILock|2|Aktiviert den Schutz von Anmeldeinformationen ohne UEFI-Sperre.|




