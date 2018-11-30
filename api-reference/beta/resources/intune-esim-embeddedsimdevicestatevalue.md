---
title: EmbeddedSIMDeviceStateValue Enum-Typ
description: Beschreibt die verschiedenen Zustände für einen eingebetteten SIM Aktivierungscode.
ms.openlocfilehash: c0b1cffedcae18dab4c1d23a2691cafa8709c0ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059255"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>EmbeddedSIMDeviceStateValue Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Beschreibt die verschiedenen Zustände für einen eingebetteten SIM Aktivierungscode.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|notEvaluated|0|Legt fest, dass der eingebettete SIM Aktivierungscode kostenlosen und verfügbar ist, ein Gerät zugewiesen werden soll.|
|failed|1|Legt fest, dass Intune Service konnte nicht an einem Gerät dieses Profil übermitteln.|
|Installieren von|2|Legt fest, dass der eingebettete SIM Aktivierungscode zu einem Gerät zugewiesen wurde, und das Gerät wird das Token installieren.|
|installiert|3|Legt fest, dass der eingebettete SIM Aktivierungscode auf das Zielgerät erfolgreich installiert wurde.|
|Löschen|4|Legt fest, dass Intune Service versucht, um das Profil vom Gerät zu löschen.|
|error|5|Legt fest, dass Fehler mit diesem Profil vorhanden ist.|
|gelöscht|6|Legt fest, dass das Profil vom Gerät gelöscht wird.|
|removedByUser|7|Legt fest, dass das Profil des Benutzers vom Gerät entfernt wird|





