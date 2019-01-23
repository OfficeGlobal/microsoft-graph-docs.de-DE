---
title: EmbeddedSIMDeviceStateValue Enum-Typ
description: Beschreibt die verschiedenen Zustände für einen eingebetteten SIM Aktivierungscode.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2da255ef2d0cf192dd09a6351bbd337f3cd9b5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421326"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>EmbeddedSIMDeviceStateValue Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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




