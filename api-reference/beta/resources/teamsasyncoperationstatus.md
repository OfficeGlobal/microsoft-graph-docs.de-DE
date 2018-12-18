---
title: TeamsAsyncOperationStatus Enum-Typ
description: Wird den aktuellen Status der ein TeamsAsyncOperation beschrieben.
author: nkramer
ms.openlocfilehash: 49b5b81999714627b1a1acd42df208594123b262
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332004"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>TeamsAsyncOperationStatus Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Wird den aktuellen Status der ein [TeamsAsyncOperation](teamsasyncoperation.md)beschrieben.

## <a name="members"></a>Elemente

| Member | Wert| Beschreibung |
|:---------------|:--------|:----------|
|Ungültig|0|Ungültiger Wert.|
|nicht gestartet|1|Der Vorgang wurde nicht gestartet.|
|in Bearbeitung|2|Der Vorgang wird ausgeführt.|
|succeeded|3|Der Vorgang erfolgreich war.|
|failed|4|Dieser Vorgang ist fehlgeschlagen.|