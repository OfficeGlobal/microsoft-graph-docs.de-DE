---
title: SecureAssessmentAccountType Enum-Typ
description: Typ der Konten, die für Windows10SecureAssessment ConfigurationAccount zulässig sind.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2f9e620f87173708b852bd7eac79bee5a45e432c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409881"
---
# <a name="secureassessmentaccounttype-enum-type"></a>SecureAssessmentAccountType Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Typ der Konten, die für Windows10SecureAssessment ConfigurationAccount zulässig sind.

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|azureADAccount|0|Gibt ein Azure AD-Konto im Format von AzureAD\ username@tenant.com an.|
|domainAccount|1|Gibt ein Domänenkonto, das im Format Domäne\Benutzer oder user@domain.com an.|
|localAccount|2|Gibt ein lokales Konto im Username-Format an.|




