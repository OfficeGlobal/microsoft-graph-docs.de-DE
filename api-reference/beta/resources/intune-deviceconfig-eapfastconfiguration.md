---
title: EapFastConfiguration Enum-Typ
description: Verfügbaren Einstellungen für EAP-FAST-Konfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 65165929d388ed57f2651a0d277996e56d2f046e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954456"
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





