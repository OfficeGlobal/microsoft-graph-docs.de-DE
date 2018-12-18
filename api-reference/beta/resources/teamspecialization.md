---
title: TeamSpecialization Enum-Typ
description: Beschreibt den speziellen Anwendungsfall für ein Team.
author: nkramer
ms.openlocfilehash: 2e17f03374457ff8ddd9d3941eb56bebbec2dde6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348013"
---
# <a name="teamspecialization-enum-type"></a>TeamSpecialization Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Gibt an, ob das [Team](../resources/team.md) für einen bestimmten Anwendungsfall vorgesehen ist. Jedes [Team](../resources/team.md) Spezialisierung hat Zugriff zur eindeutigen Verhalten und seine Anwendungsfall Ziel Erfahrungen. Standardwert ist "none".

## <a name="members"></a>Elemente

| Member             | Wert | Beschreibung                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| Keine               | 0     | Standard-Typ für ein Team die die standard-Team-Erfahrung haben.          |
| unknownFutureValue | 7     | Sentinel Wert als Platzhalter für zukünftige Erweiterung der Enumeration reserviert. |
