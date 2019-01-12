---
title: LocalSecurityOptionsMinimumSessionSecurity Enum-Typ
description: Mögliche Werte für LocalSecurityOptionsMinimumSessionSecurity
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 822c996d788fd5edb5c92f876c725b771b051c15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952482"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>LocalSecurityOptionsMinimumSessionSecurity Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für LocalSecurityOptionsMinimumSessionSecurity
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|n/v|0|LM & NTLM-Antworten senden|
|requireNtmlV2SessionSecurity|1|Senden Sie LM & NTLM-Verwendung NTLMv2 sitzungssicherheit, wenn ausgehandelt|
|require128BitEncryption|2|LM & NTLM-Antworten senden|
|ntlmV2And128BitEncryption|3|LM & NTLMv2-Antworten senden|





