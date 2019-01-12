---
title: TeamSpecialization Enum-Typ
description: Beschreibt den speziellen Anwendungsfall für ein Team.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a2272ee085d0c265adc9ce2e3f1c598e45be21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930285"
---
# <a name="teamspecialization-enum-type"></a>TeamSpecialization Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Gibt an, ob das [Team](../resources/team.md) für einen bestimmten Anwendungsfall vorgesehen ist. Jedes [Team](../resources/team.md) Spezialisierung hat Zugriff zur eindeutigen Verhalten und seine Anwendungsfall Ziel Erfahrungen. Standardwert ist "none".

## <a name="members"></a>Elemente

| Element             | Wert | Beschreibung                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| n/v               | 0     | Standard-Typ für ein Team die die standard-Team-Erfahrung haben.          |
| unknownFutureValue | 7     | Sentinel Wert als Platzhalter für zukünftige Erweiterung der Enumeration reserviert. |
