---
title: EapFastConfiguration Enum-Typ
description: Verfügbaren Einstellungen für EAP-FAST-Konfiguration.
ms.openlocfilehash: b1771668ea627d2e873d54334e388989652736d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060567"
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





