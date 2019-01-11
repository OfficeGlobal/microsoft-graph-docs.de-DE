---
title: SecureAssessmentAccountType Enum-Typ
description: Typ der Konten, die für Windows10SecureAssessment ConfigurationAccount zulässig sind.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5b1f8a3d03c0e7b9e91c68ff5a87611fcaa6f31e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826054"
---
# <a name="secureassessmentaccounttype-enum-type"></a>SecureAssessmentAccountType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Typ der Konten, die für Windows10SecureAssessment ConfigurationAccount zulässig sind.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|azureADAccount|0|Gibt ein Azure AD-Konto im Format von AzureAD\ username@tenant.com an.|
|domainAccount|1|Gibt ein Domänenkonto, das im Format Domäne\Benutzer oder user@domain.com an.|
|localAccount|2|Gibt ein lokales Konto im Username-Format an.|





