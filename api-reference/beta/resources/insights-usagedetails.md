---
title: Ressourcentyp usageDetails
description: Komplexer Typ, die Eigenschaften des verwendeten Elemente enthält. Wenn die Ressource des letzten Zugriffs auf Informationen (Ansicht) und (bearbeitet) vom Benutzer geändert.
author: simonhult
ms.openlocfilehash: ef5efcfce439e9d08784637cb02657d7cd37adf7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349350"
---
# <a name="usagedetails-resource-type"></a>Ressourcentyp usageDetails

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Komplexer Typ, enthält die Eigenschaften von Elementen [verwendet](insights-used.md) . Wenn die Ressource des letzten Zugriffs auf Informationen (Ansicht) und (bearbeitet) vom Benutzer geändert.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft              | Typ          | Beschreibung  |
| -------------         |---------------| -------------|
| lastAccessedDateTime                  | DateTimeOffset        | Das Datum und die Zeit, die die Ressource zuletzt vom Benutzer zugegriffen werden konnte. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`. Schreibgeschützt.                      |
| lastModifiedDateTime              | DateTimeOffset        | Datum und Uhrzeit der letzten Änderung die Ressource durch den Benutzer. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`. Schreibgeschützt.       |