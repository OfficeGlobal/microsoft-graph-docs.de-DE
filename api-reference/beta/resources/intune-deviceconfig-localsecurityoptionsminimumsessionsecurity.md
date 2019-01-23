---
title: LocalSecurityOptionsMinimumSessionSecurity Enum-Typ
description: Mögliche Werte für LocalSecurityOptionsMinimumSessionSecurity
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c39f2bb6d0bab2aff09fc05bb0492e81102e1b7c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396084"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a>LocalSecurityOptionsMinimumSessionSecurity Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Mögliche Werte für LocalSecurityOptionsMinimumSessionSecurity

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|Keine|0|LM & NTLM-Antworten senden|
|requireNtmlV2SessionSecurity|1|Senden Sie LM & NTLM-Verwendung NTLMv2 sitzungssicherheit, wenn ausgehandelt|
|require128BitEncryption|2|LM & nur NTLM-Antworten senden|
|ntlmV2And128BitEncryption|3|LM & nur NTLMv2-Antworten senden|




