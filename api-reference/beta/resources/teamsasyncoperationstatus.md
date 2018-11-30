---
title: TeamsAsyncOperationStatus Enum-Typ
description: Wird den aktuellen Status der ein TeamsAsyncOperation beschrieben.
ms.openlocfilehash: f553242ace983651b8d4fda77370de712f9d08b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059097"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>TeamsAsyncOperationStatus Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Wird den aktuellen Status der ein [TeamsAsyncOperation](teamsasyncoperation.md)beschrieben.

## <a name="members"></a>Elemente

| Element | Wert| Beschreibung |
|:---------------|:--------|:----------|
|Ungültig|0|Ungültiger Wert.|
|nicht gestartet|1|Der Vorgang wurde nicht gestartet.|
|in Bearbeitung|2|Der Vorgang wird ausgeführt.|
|succeeded|3|Der Vorgang erfolgreich war.|
|failed|4|Dieser Vorgang ist fehlgeschlagen.|