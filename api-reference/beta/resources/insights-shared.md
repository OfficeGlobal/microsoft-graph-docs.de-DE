---
title: freigegebene Ressource-Typ
description: 'Einen Einblick, freigegebene mit oder von einem bestimmten Benutzer Dateien darstellt. Die folgenden freigegebenen Dateien werden unterstützt:'
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 289523f836d7b8080f7317e4d11301c71314ba93
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880612"
---
# <a name="shared-resource-type"></a>freigegebene Ressource-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Einen Einblick, freigegebene mit oder von einem bestimmten Benutzer Dateien darstellt. Die folgenden freigegebenen Dateien werden unterstützt:

- Anlagen direkt in eine e-Mail oder eine Besprechung einladen.
- OneDrive für Bussiness und SharePoint modernen Anlagen - Dateien in OneDrive für Unternehmen und SharePoint, die Benutzer in einer e-Mail als ein Links freigeben.

**Hinweis**: Wir arbeiten derzeit auf die Ergebnisse der Shared-API mit Daten auffüllen. Möglicherweise gibt es einige Daten in den ersten Wochen nach der Veröffentlichung fehlt.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Gemeinsame Liste](../api/insights-list-shared.md) |[Insights_shared](insights-shared.md) -Auflistung| Rufen Sie eine Liste der freigegebenen Dateien.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft              | Typ                      | Beschreibung  |
| -------------         |---------------            | -------------|
| id                    | Zeichenfolge                    | Eindeutiger Bezeichner der Beziehung. Schreibgeschützt.        |
| lastShared            | [sharingDetail](insights-sharingdetail.md)                | Informationen zu freigegebenen Elements. Schreibgeschützt.        |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Eigenschaften, die Sie verwenden können, um das Dokument in Ihre Erfahrung visualisieren. Schreibgeschützt.      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Referenz-Eigenschaften des freigegebenen Dokuments, wie die Url und den Typ des Dokuments. Schreibgeschützt.       |

## <a name="relationships"></a>Beziehungen

| Eigenschaft      | Typ          | Beschreibung  |
| ------------- |---------------| -------------|
| resource      | Entität        | Verwendet zum Navigieren zu dem Element, das freigegeben wurde. Dateianlagen ist der Typ *FileAttachment*. Für verknüpfte Anlagen ist der Typ *DriveItem*. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
