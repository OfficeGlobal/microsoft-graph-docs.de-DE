---
title: Mitglieder
description: Wird den aktuelle Installationsstatus von einer TeamsApp beschrieben.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 4e453a28b0c3ebc2957cf7e1a92a846e8e4758e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847572"
---
#<a name="teamsappinstalledstate-enum-type"></a>TeamsAppInstalledState Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Wird den aktuelle Installationsstatus von einer [TeamsApp](teamsapp.md)beschrieben.

## <a name="members"></a>Elemente

| Element | Wert| Beschreibung |
|:---------------|:--------|:----------|
|notInstalled|0|App wird an das Team nicht installiert.|
|installiert|1|App wird normalerweise installiert.|
|installedAndHidden|2|App wird installiert, jedoch ausgeblendet.|
|installedAndPermanent|3|App wird dauerhaft installiert und kann nicht entfernt werden.|
