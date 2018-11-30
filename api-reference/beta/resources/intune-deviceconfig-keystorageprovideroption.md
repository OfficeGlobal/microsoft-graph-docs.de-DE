---
title: KeyStorageProviderOption Enum-Typ
description: Importoptionen für wichtige Speicher-Anbieter (KSP).
ms.openlocfilehash: 236489d288ec0be70a818e1c51b8c634ad3933a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059042"
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





