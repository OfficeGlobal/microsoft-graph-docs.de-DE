---
title: KeyStorageProviderOption Enum-Typ
description: Importoptionen für wichtige Speicher-Anbieter (KSP).
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f3a8169b4bb6cd2357f02aa7fec89ba640780f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946553"
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





