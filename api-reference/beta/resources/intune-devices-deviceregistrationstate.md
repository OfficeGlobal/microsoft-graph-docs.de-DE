---
title: DeviceRegistrationState Enum-Typ
description: Registrierung Gerätestatus.
author: tfitzmac
ms.openlocfilehash: a622613bd4ca5e065c3d9eb0331c05c360c1837c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360543"
---
# <a name="deviceregistrationstate-enum-type"></a>DeviceRegistrationState Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Registrierung Gerätestatus.
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|nicht registriert|0|Das Gerät ist nicht registriert.|
|registriert|2|Das Gerät registriert ist.|
|widerrufen|3|Das Gerät wurde blockiert, gelöscht oder zurückgezogen.|
|keyConflict|4|Das Gerät hat einen Konflikt mit Schlüssel.|
|approvalPending|5|Das Gerät ist ausstehender Genehmigung.|
|certificateReset|6|Das Gerät Zertifikat wurde zurückgesetzt.|
|notRegisteredPendingEnrollment|7|Das Gerät ist nicht registriert und ausstehenden Registrierung.|
|unknown|8|Die Registrierung Gerätestatus ist unbekannt.|





