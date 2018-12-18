---
title: EmbeddedSIMDeviceStateValue Enum-Typ
description: Beschreibt die verschiedenen Zustände für einen eingebetteten SIM Aktivierungscode.
author: tfitzmac
ms.openlocfilehash: 51e550669d9cd29d7d5bb246fe2cba017b02187c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320594"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>EmbeddedSIMDeviceStateValue Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Beschreibt die verschiedenen Zustände für einen eingebetteten SIM Aktivierungscode.
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|notEvaluated|0|Legt fest, dass der eingebettete SIM Aktivierungscode kostenlosen und verfügbar ist, ein Gerät zugewiesen werden soll.|
|failed|1|Legt fest, dass Intune Service konnte nicht an einem Gerät dieses Profil übermitteln.|
|Installieren von|2|Legt fest, dass der eingebettete SIM Aktivierungscode zu einem Gerät zugewiesen wurde, und das Gerät wird das Token installieren.|
|installiert|3|Legt fest, dass der eingebettete SIM Aktivierungscode auf das Zielgerät erfolgreich installiert wurde.|
|Löschen|4|Legt fest, dass Intune Service versucht, um das Profil vom Gerät zu löschen.|
|error|5|Legt fest, dass Fehler mit diesem Profil vorhanden ist.|
|gelöscht|6|Legt fest, dass das Profil vom Gerät gelöscht wird.|
|removedByUser|7|Legt fest, dass das Profil des Benutzers vom Gerät entfernt wird|





