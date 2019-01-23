---
title: KeyStorageProviderOption Enum-Typ
description: Importoptionen für wichtige Speicher-Anbieter (KSP).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6993d7e241ef94c572975c709c286a14f6eabf5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424224"
---
# <a name="keystorageprovideroption-enum-type"></a>KeyStorageProviderOption Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Importoptionen für wichtige Speicher-Anbieter (KSP).

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|Importieren Sie um Modul TPM (Trusted Platform) KSP, falls vorhanden, andernfalls in Software KSP importieren.|
|useTpmKspOtherwiseFail|1|Import auf Modul TPM (Trusted Platform) KSP, falls vorhanden, andernfalls ein Fehler auftritt.|
|usePassportForWorkKspOtherwiseFail|2|Importieren von Passport für Arbeit KSP falls verfügbar, andernfalls ein Fehler auftritt.|
|useSoftwareKsp|3|In Software KSP importieren.|




