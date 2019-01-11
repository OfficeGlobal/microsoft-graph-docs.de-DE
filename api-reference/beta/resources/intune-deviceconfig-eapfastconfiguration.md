---
title: EapFastConfiguration Enum-Typ
description: Verfügbaren Einstellungen für EAP-FAST-Konfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 499d6595980bcb6bca1ea93687399e8988a3bed7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811088"
---
# <a name="eapfastconfiguration-enum-type"></a>EapFastConfiguration Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Verfügbaren Einstellungen für EAP-FAST-Konfiguration.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|noProtectedAccessCredential|0|EAP-FAST ohne geschützte Zugriffsberechtigung (PAC) verwenden.|
|useProtectedAccessCredential|1|Verwenden Sie geschützte Zugriffsinformationen (PAC).|
|useProtectedAccessCredentialAndProvision|2|Verwendung geschützt Access Anmeldeinformationen (PAC) und Provision PAC|
|useProtectedAccessCredentialAndProvisionAnonymously|3|Verwenden Sie geschützte Zugriffsberechtigung (PAC), PAC bereitgestellt werden soll, und dazu anonym.|





