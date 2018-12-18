---
title: LanManagerAuthenticationLevel Enum-Typ
description: Mögliche Werte für LanManagerAuthenticationLevel
author: tfitzmac
ms.openlocfilehash: fd5d63f262b9b6e9a27060725e721cb81c495a57
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308743"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>LanManagerAuthenticationLevel Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für LanManagerAuthenticationLevel
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|lmAndNltm|0|LM & NTLM-Antworten senden|
|lmNtlmAndNtlmV2|1|Senden Sie LM & NTLM-Verwendung NTLMv2 sitzungssicherheit, wenn ausgehandelt|
|lmAndNtlmOnly|2|LM & NTLM-Antworten senden|
|lmAndNtlmV2|3|LM & NTLMv2-Antworten senden|
|lmNtlmV2AndNotLm|4|Senden Sie nur LM & NTLMv2-Antworten. LM verweigern|
|lmNtlmV2AndNotLmOrNtm|5|Senden Sie nur LM & NTLMv2-Antworten. LM NTLM verweigern|





