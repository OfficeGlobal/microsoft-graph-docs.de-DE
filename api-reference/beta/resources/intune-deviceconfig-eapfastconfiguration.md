---
title: EapFastConfiguration Enum-Typ
description: Verfügbaren Einstellungen für EAP-FAST-Konfiguration.
author: tfitzmac
ms.openlocfilehash: ba84adb86e9910df47bd236fd2bd348cbc9c8e6f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326362"
---
# <a name="eapfastconfiguration-enum-type"></a>EapFastConfiguration Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Verfügbaren Einstellungen für EAP-FAST-Konfiguration.
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|noProtectedAccessCredential|0|EAP-FAST ohne geschützte Zugriffsberechtigung (PAC) verwenden.|
|useProtectedAccessCredential|1|Verwenden Sie geschützte Zugriffsinformationen (PAC).|
|useProtectedAccessCredentialAndProvision|2|Verwendung geschützt Access Anmeldeinformationen (PAC) und Provision PAC|
|useProtectedAccessCredentialAndProvisionAnonymously|3|Verwenden Sie geschützte Zugriffsberechtigung (PAC), PAC bereitgestellt werden soll, und dazu anonym.|





