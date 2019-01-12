---
title: LanManagerAuthenticationLevel Enum-Typ
description: Mögliche Werte für LanManagerAuthenticationLevel
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fd88deb7684301023a75905d12a59ce25bad750f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911994"
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





