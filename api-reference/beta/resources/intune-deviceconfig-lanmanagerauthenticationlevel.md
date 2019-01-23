---
title: LanManagerAuthenticationLevel Enum-Typ
description: Mögliche Werte für LanManagerAuthenticationLevel
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6e8c7b3df6f515d3dad0d7619b6c0b755ad799d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397456"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>LanManagerAuthenticationLevel Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Mögliche Werte für LanManagerAuthenticationLevel

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|lmAndNltm|0|LM & NTLM-Antworten senden|
|lmNtlmAndNtlmV2|1|Senden Sie LM & NTLM-Verwendung NTLMv2 sitzungssicherheit, wenn ausgehandelt|
|lmAndNtlmOnly|2|LM & nur NTLM-Antworten senden|
|lmAndNtlmV2|3|LM & nur NTLMv2-Antworten senden|
|lmNtlmV2AndNotLm|4|Senden Sie LM & nur die NTLMv2-Antworten. LM verweigern|
|lmNtlmV2AndNotLmOrNtm|5|Senden Sie LM & nur die NTLMv2-Antworten. LM & NTLM verweigern|




