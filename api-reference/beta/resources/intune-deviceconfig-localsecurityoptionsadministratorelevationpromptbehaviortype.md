---
title: LocalSecurityOptionsAdministratorElevationPromptBehaviorType Enum-Typ
description: Mögliche Werte für LocalSecurityOptionsAdministratorElevationPromptBehavior
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ae886f6c7696150cb85a17cb2caa65823705e121
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916824"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a>LocalSecurityOptionsAdministratorElevationPromptBehaviorType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für LocalSecurityOptionsAdministratorElevationPromptBehavior
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|nicht konfiguriert|0|Nicht konfiguriert|
|elevateWithoutPrompting|1|Zu erhöhen, ohne aufzufordern.|
|promptForCredentialsOnTheSecureDesktop|2|Aufforderung zur erneuten Eingabe auf dem sicheren desktop|
|promptForConsentOnTheSecureDesktop|3|Aufforderung zur Bestätigung auf dem sicheren desktop|
|promptForCredentials|4|Aufforderung zur erneuten Eingabe|
|promptForConsent|5|Aufforderung zur Bestätigung|
|promptForConsentForNonWindowsBinaries|6|Aufforderung zur Bestätigung für nicht-Windows-Binärdateien|





