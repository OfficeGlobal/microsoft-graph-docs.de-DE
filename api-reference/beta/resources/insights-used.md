---
title: Ressourcentyp verwendet
description: Einen Einblick, Dokumente, die von einem bestimmten Benutzer darstellt. Einblicke in die gibt, die zutreffenden Dokumente, die ein Benutzer anzeigen oder darauf zugreifen.
author: simonhult
ms.openlocfilehash: 89eac33ad954905c77a26df669bb15a2cf471edd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323485"
---
# <a name="used-resource-type"></a>Ressourcentyp verwendet

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Einen Einblick, Dokumente, die von einem bestimmten Benutzer darstellt. Einblicke in die gibt, die zutreffenden Dokumente, die ein Benutzer anzeigen oder darauf zugreifen. Dazu gehören Dokumente in:

- OneDrive for Business
- SharePoint

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Verwendet wird](../api/insights-list-used.md) |[Insights_used](insights-used.md) -Auflistung| Rufen Sie eine Liste der geöffneten Dateien.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft              | Typ                      | Beschreibung  |
| -------------         |---------------            | -------------|
| id                    | String                    | Eindeutiger Bezeichner der Beziehung. Schreibgeschützt.        |
| lastUsed              | [usageDetails](insights-usagedetails.md)              | Wenn das Element zuletzt Informationen angezeigt und vom Benutzer geändert. Schreibgeschützt.     |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Eigenschaften, die Sie verwenden können, um das Dokument in Ihre Erfahrung visualisieren. Schreibgeschützt.      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Referenz-Eigenschaften des Dokuments verwendete, wie die Url und den Typ des Dokuments. Schreibgeschützt.     |

## <a name="relationships"></a>Beziehungen

| Eigenschaft      | Typ          | Beschreibung  |
| ------------- |---------------| -------------|
| resource      | Entität        | Verwendet zum Navigieren zu dem Element, das verwendet wurde. Dateianlagen ist der Typ *FileAttachment*. Für verknüpfte Anlagen ist der Typ *DriveItem*. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```