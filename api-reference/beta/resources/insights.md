---
title: Einblicke in die Ressourcentyp
description: Einblicke in die sind Beziehungen mit erweiterten Analyse- und Techniken erlernen Computer berechnet. Sie können, zum Beispiel OneDrive Dokumente, um Benutzer Trend identifizieren.
author: simonhult
ms.openlocfilehash: f3269134f4a80462359a11d603c3f843be0c62f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318599"
---
# <a name="insights-resource-type"></a>Einblicke in die Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Einblicke in die sind Beziehungen mit erweiterten Analyse- und Techniken erlernen Computer berechnet. Sie können, zum Beispiel OneDrive Dokumente, um Benutzer Trend identifizieren.

Einblicke in die werden durch die folgenden APIs zurückgegeben:

- [Trending](insights-trending.md) - gibt Dokumente aus OneDrive und aus SharePoint-Websites, um einen Benutzer Trend zurück.
- [Used](insights-used.md) - gibt Dokumente angezeigt und geändert werden, von einem Benutzer zurück. Enthält Dokumente, die der Benutzer verwendet in OneDrive für Unternehmen, SharePoint, als e-Mail-Anlagen und als Link Anlagen aus Quellen wie Feld, Ablage und Google Laufwerk geöffnet wurde.
- [Shared](insights-shared.md) - gibt mit einem Benutzer freigegebene Dokumente zurück. Dokumente können als e-Mail-Anlage oder als OneDrive freigegeben werden for Business in gesendete e-Mails verknüpft.

Jede Erkenntnisse wird zurückgegeben, mit einer `resourceVisualization` und `resourceReference` komplexe Werttyp (CVT). Die ResourceVisualization CVT enthält Eigenschaften wie `title` und `previewImageUrl`. Microsoft verwendet die Visualisierungseigenschaften zum Rendern von Dateien im Erfahrungen wie Office ausführlicher behandelt.

## <a name="relationships"></a>Beziehungen

| Beziehung      | Typ          | Beschreibung  |
| ------------- |---------------| -------------|
| Trend      | [Trending](insights-trending.md) -Auflistung       | Berechnete Beziehung Identifizieren von Trend Dokumenten. Trend Dokumente können in OneDrive oder in SharePoint-Websites gespeichert werden.   |
| verwendet      | [Used](insights-used.md) -Auflistung       | Identifizieren von Dokumenten angezeigt und geändert werden, von einem Benutzer Beziehung berechnet. Enthält Dokumente, die der Benutzer verwendet in OneDrive für Unternehmen, SharePoint, als e-Mail-Anlagen und als Link Anlagen aus Quellen wie Feld, Ablage und Google Laufwerk geöffnet wurde.  |
| shared        | [Shared](insights-shared.md) -Auflistung       | Berechnete Beziehung Identifizieren von Dokumenten, die ein Benutzer freigegeben. Dokumente können als e-Mail-Anlage oder als OneDrive freigegeben werden for Business in gesendete e-Mails verknüpft.   |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.
```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```