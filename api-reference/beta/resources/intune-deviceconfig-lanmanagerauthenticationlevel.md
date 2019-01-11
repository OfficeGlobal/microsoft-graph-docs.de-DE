---
title: LanManagerAuthenticationLevel Enum-Typ
description: Mögliche Werte für LanManagerAuthenticationLevel
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 68af209a005dc1d7e8d25672f5e97e1d929ba25b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866913"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>LanManagerAuthenticationLevel Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für LanManagerAuthenticationLevel
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|lmAndNltm|0|LM & NTLM-Antworten senden|
|lmNtlmAndNtlmV2|1|Senden Sie LM & NTLM-Verwendung NTLMv2 sitzungssicherheit, wenn ausgehandelt|
|lmAndNtlmOnly|2|LM & NTLM-Antworten senden|
|lmAndNtlmV2|3|LM & NTLMv2-Antworten senden|
|lmNtlmV2AndNotLm|4|Senden Sie nur LM & NTLMv2-Antworten. LM verweigern|
|lmNtlmV2AndNotLmOrNtm|5|Senden Sie nur LM & NTLMv2-Antworten. LM NTLM verweigern|





