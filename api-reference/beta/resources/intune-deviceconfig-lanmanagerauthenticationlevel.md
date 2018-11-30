---
title: LanManagerAuthenticationLevel Enum-Typ
description: Mögliche Werte für LanManagerAuthenticationLevel
ms.openlocfilehash: 9fb8113c4953a0cabcecfbc5303b9f62f685d5ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058611"
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





