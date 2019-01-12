---
title: SecureAssessmentAccountType Enum-Typ
description: Typ der Konten, die für Windows10SecureAssessment ConfigurationAccount zulässig sind.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9e5ae78b5df3636e738cf21beece269e6fa7b81a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959258"
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





