---
title: Ressourcentyp sharingDetail
description: 'Komplexer Typ, der Eigenschaften von gemeinsamen Elementen enthält. '
author: simonhult
ms.openlocfilehash: 8454fd451f0659ff3ccad270df3414a850bee180
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353375"
---
# <a name="sharingdetail-resource-type"></a>Ressourcentyp sharingDetail

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Komplexer Typ, der Eigenschaften von [gemeinsamen](insights-shared.md) Elementen enthält. 

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft              | Typ          | Beschreibung  |
| -------------         |-----------    | -------------|
| sharedDateTime        | DateTimeOffset| Das Datum und die Zeit, die die Datei zuletzt freigegeben wurde. Der Zeitstempel stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`. Schreibgeschützt.  |
| sharingSubject        | String          | Der Betreff, mit dem das Dokument freigegeben wurde. |
| sharingType             | String        | Bestimmt, wie das Dokument freigegeben wurde, kann durch "Link", "Anlage", "Group", "Site" sein.     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | Der Benutzer, die das Dokument freigegeben.  |
| sharingReference        | [resourceReference](insights-resourcereference.md)      |  |