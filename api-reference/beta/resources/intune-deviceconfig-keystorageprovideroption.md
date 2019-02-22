---
title: keyStorageProviderOption-Enumerationstyp
description: Import Optionen des Schlüsselspeicheranbieters (KSP).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ddc1cffe1f4e6056d53a151a3b36b2622c9bf4b5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153018"
---
# <a name="keystorageprovideroption-enum-type"></a>keyStorageProviderOption-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Import Optionen des Schlüsselspeicheranbieters (KSP).

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|useTpmKspOtherwiseUseSoftwareKsp|0|Import in Trusted Platform Module (TPM) KSP, falls vorhanden, andernfalls in Software KSP importieren.|
|useTpmKspOtherwiseFail|1|Importieren Sie in Trusted Platform Module (TPM) KSP, falls vorhanden, andernfalls fehlschlagen.|
|usePassportForWorkKspOtherwiseFail|2|Import in Passport für Arbeit KSP, falls verfügbar, andernfalls fehlschlagen.|
|useSoftwareKsp|3|Importieren in Software KSP.|




