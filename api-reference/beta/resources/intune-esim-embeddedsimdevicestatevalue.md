---
title: EmbeddedSIMDeviceStateValue Enum-Typ
description: Beschreibt die verschiedenen Zustände für einen eingebetteten SIM Aktivierungscode.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a3974c0df65ef9f59242f390b7166e11c3e0c592
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886058"
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





