---
title: Mitglieder
description: Wird den aktuelle Installationsstatus von einer TeamsApp beschrieben.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ca42b56e2c374dbaea1df676e3a84569b192e78c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937173"
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
