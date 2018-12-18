---
title: SecureAssessmentAccountType Enum-Typ
description: Typ der Konten, die für Windows10SecureAssessment ConfigurationAccount zulässig sind.
author: tfitzmac
ms.openlocfilehash: faf504410336bdc491c29b676aaa1b57cd0a5ee2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362223"
---
# <a name="secureassessmentaccounttype-enum-type"></a>SecureAssessmentAccountType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Typ der Konten, die für Windows10SecureAssessment ConfigurationAccount zulässig sind.
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|azureADAccount|0|Gibt ein Azure AD-Konto im Format von AzureAD\ username@tenant.com an.|
|domainAccount|1|Gibt ein Domänenkonto, das im Format Domäne\Benutzer oder user@domain.com an.|
|localAccount|2|Gibt ein lokales Konto im Username-Format an.|





