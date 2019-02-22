---
title: localSecurityOptionsMinimumSessionSecurity-Enumerationstyp
description: Mögliche Werte für LocalSecurityOptionsMinimumSessionSecurity
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe6007747aed1037a4dc3d5264bb432182a28c00
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145346"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>localSecurityOptionsMinimumSessionSecurity-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Mögliche Werte für LocalSecurityOptionsMinimumSessionSecurity

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|Keine|0|Senden von LM-& NTLM-Antworten|
|requireNtmlV2SessionSecurity|1|Senden von LM-& NTLM-Verwendung der NTLMv2-Sitzungssicherheit bei aushandeln|
|require128BitEncryption|2|Nur nur NTLM-Antworten für LM-& senden|
|ntlmV2And128BitEncryption|3|Nur LM-&-NTLMv2-Antworten senden|




