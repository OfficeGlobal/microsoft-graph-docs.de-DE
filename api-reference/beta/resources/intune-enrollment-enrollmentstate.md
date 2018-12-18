---
title: EnrollmentState Enum-Typ
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 5e432f73ace1adbd529c910f70b97b7357a406e3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301295"
---
# <a name="enrollmentstate-enum-type"></a>EnrollmentState Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Die Registrierung des Geräts ist unbekannt|
|registriert|1|Gerät ist registriert.|
|pendingReset|2|Registriert, aber es über Registrierung Profil registriert ist und das registrierte Profil unterscheidet sich von der zugewiesenen Profil.|
|failed|3|Nicht registriert und Registrierung Fehler Datensatz vorhanden ist.|
|notContacted|4|Gerät ist importiert, aber nicht registriert.|
|gesperrt|5|Gerät als userless registriert ist, aber wird blockiert zu Benutzer Registrierung navigieren, da die app konnte nicht installiert werden.|





