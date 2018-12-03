---
title: Elemente
description: Wird den aktuelle Installationsstatus von einer TeamsApp beschrieben.
ms.openlocfilehash: 7f358a621a25219e78e3a02ce081d07a27395d2c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064004"
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
