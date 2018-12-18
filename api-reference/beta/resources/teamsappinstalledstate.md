---
title: Members
description: Wird den aktuelle Installationsstatus von einer TeamsApp beschrieben.
author: nkramer
ms.openlocfilehash: a73c68298c4cdf65deee68fb3bd707d50bc2475a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316793"
---
#<a name="teamsappinstalledstate-enum-type"></a>TeamsAppInstalledState Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Wird den aktuelle Installationsstatus von einer [TeamsApp](teamsapp.md)beschrieben.

## <a name="members"></a>Elemente

| Member | Wert| Beschreibung |
|:---------------|:--------|:----------|
|notInstalled|0|App wird an das Team nicht installiert.|
|installiert|1|App wird normalerweise installiert.|
|installedAndHidden|2|App wird installiert, jedoch ausgeblendet.|
|installedAndPermanent|3|App wird dauerhaft installiert und kann nicht entfernt werden.|
