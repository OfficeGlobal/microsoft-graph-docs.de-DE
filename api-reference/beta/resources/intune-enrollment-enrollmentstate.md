---
title: EnrollmentState Enum-Typ
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9394755c5b6e6de8ed039b226d03074f1ef16cc3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933589"
---
# <a name="enrollmentstate-enum-type"></a>EnrollmentState Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|unknown|0|Die Registrierung des Geräts ist unbekannt|
|registriert|1|Gerät ist registriert.|
|pendingReset|2|Registriert, aber es über Registrierung Profil registriert ist und das registrierte Profil unterscheidet sich von der zugewiesenen Profil.|
|failed|3|Nicht registriert und Registrierung Fehler Datensatz vorhanden ist.|
|notContacted|4|Gerät ist importiert, aber nicht registriert.|
|gesperrt|5|Gerät als userless registriert ist, aber wird blockiert zu Benutzer Registrierung navigieren, da die app konnte nicht installiert werden.|





