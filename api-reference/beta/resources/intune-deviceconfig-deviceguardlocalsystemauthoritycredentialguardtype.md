---
title: DeviceGuardLocalSystemAuthorityCredentialGuardType Enum-Typ
description: Mögliche Werte von Anmeldeinformationen Guard-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d284b81632c5ba48fa4c658719203a74fdf52837
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952741"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a>DeviceGuardLocalSystemAuthorityCredentialGuardType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte von Anmeldeinformationen Guard-Einstellungen.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|nicht konfiguriert|0|Schaltet Anmeldeinformationen Guard Remote Wenn zuvor ohne UEFI Sperre konfiguriert.|
|enableWithUEFILock|1|Aktiviert die Anmeldeinformationen Guard mit UEFI sperren.|
|enableWithoutUEFILock|2|Aktiviert die Anmeldeinformationen Guard ohne UEFI sperren.|





