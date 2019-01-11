---
title: KeyStorageProviderOption Enum-Typ
description: Importoptionen für wichtige Speicher-Anbieter (KSP).
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4609092c3022b62331bbb6226a5b91e4b287ff79
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826467"
---
# <a name="keystorageprovideroption-enum-type"></a>KeyStorageProviderOption Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Importoptionen für wichtige Speicher-Anbieter (KSP).
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|Importieren Sie um Modul TPM (Trusted Platform) KSP, falls vorhanden, andernfalls in Software KSP importieren.|
|useTpmKspOtherwiseFail|1|Import auf Modul TPM (Trusted Platform) KSP, falls vorhanden, andernfalls ein Fehler auftritt.|
|usePassportForWorkKspOtherwiseFail|2|Importieren von Passport für Arbeit KSP falls verfügbar, andernfalls ein Fehler auftritt.|
|useSoftwareKsp|3|In Software KSP importieren.|





