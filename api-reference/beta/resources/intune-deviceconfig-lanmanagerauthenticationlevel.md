---
title: lanManagerAuthenticationLevel-Enumerationstyp
description: Mögliche Werte für LanManagerAuthenticationLevel
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63f04f1ef2fc12fa0352aeec803c46fb4ebab3d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166570"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a>lanManagerAuthenticationLevel-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Mögliche Werte für LanManagerAuthenticationLevel

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|lmAndNltm|0|Senden von LM-& NTLM-Antworten|
|lmNtlmAndNtlmV2|1|Senden von LM-& NTLM-Verwendung der NTLMv2-Sitzungssicherheit bei aushandeln|
|lmAndNtlmOnly|2|Nur nur NTLM-Antworten für LM-& senden|
|lmAndNtlmV2|3|Nur LM-&-NTLMv2-Antworten senden|
|lmNtlmV2AndNotLm|4|Senden Sie nur LINEARe &-NTLMv2-Antworten. LM ablehnen|
|lmNtlmV2AndNotLmOrNtm|5|Senden Sie nur LINEARe &-NTLMv2-Antworten. Ablehnen von LM & NTLM|




