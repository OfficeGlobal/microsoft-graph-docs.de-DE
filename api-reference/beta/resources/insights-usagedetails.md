---
title: Ressourcentyp usageDetails
description: Komplexer Typ, die Eigenschaften des verwendeten Elemente enthält. Wenn die Ressource des letzten Zugriffs auf Informationen (Ansicht) und (bearbeitet) vom Benutzer geändert.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 8729973c2393a918d26314ec3b27a2c68079dbfd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858954"
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
