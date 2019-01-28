---
title: insights-Ressourcentyp
description: Einblicke sind Beziehungen, die mithilfe erweiterter Analysetechniken und computergestützter Lerntechniken berechnet werden. Sie können z. B. OneDrive-Dokumente für Benutzer identifizieren.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 4e71dbca7bf4ebbe054d0da83436e5dc2129cf19
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513690"
---
# <a name="insights-resource-type"></a>insights-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Einblicke sind Beziehungen, die mithilfe erweiterter Analysetechniken und computergestützter Lerntechniken berechnet werden. Sie können z. B. OneDrive-Dokumente für Benutzer identifizieren.

Einblicke werden von den folgenden APIs zurückgegeben:

- [Trending](insights-trending.md): Gibt Dokumente von OneDrive- und SharePoint-Websites zurück, die bei einem Benutzer beliebt sind.
- [Used](insights-used.md): Gibt die zuletzt von einem Benutzer angezeigten oder geänderten Dokumente zurück. Umfasst Dokumente, die der Benutzer in OneDrive for Business und SharePoint verwendet und als E-Mail-Anlagen und als Linkanlagen von Quellen wie Box, DropBox and Google Drive geöffnet hat.
- [Shared](insights-shared.md): Gibt Dokumente zurück, die für einen Benutzer freigegeben wurden. Dokumente können als E-Mail-Anlagen oder als OneDrive for Business-Links freigegeben werden, die in E-Mails gesendet werden.

Jeder Einblick wird mit einem komplexen Werttyp von `resourceVisualization` und `resourceReference` zurückgegeben. Der komplexe Werttyp „ResourceVisualization“ enthält Eigenschaften wie `title` und `previewImageUrl`. Microsoft verwendet die Visualisierungseigenschaften, um die Dateien in Oberflächen wie Office Delve zu rendern.

## <a name="relationships"></a>Beziehungen

| Beziehung      | Typ          | Beschreibung  |
| ------------- |---------------| -------------|
| trending      | [Trending](insights-trending.md)-Auflistung       | Berechnete Beziehung, die beliebte Dokumente identifiziert. Beliebte Dokumente können auf OneDrive- oder auf SharePoint-Websites gespeichert werden.   |
| verwendet      | [Used](insights-used.md)-Auflistung       | Berechnete Beziehung, die die von einem Benutzer angezeigten und geänderten Dokumente identifiziert. Umfasst Dokumente, die der Benutzer in OneDrive for Business und SharePoint verwendet und als E-Mail-Anlagen und als Linkanlagen von Quellen wie Box, DropBox and Google Drive geöffnet hat.  |
| shared        | [Shared](insights-shared.md)-Auflistung       | Berechnete Beziehung, die Dokumente identifiziert, die für einen Benutzer freigegeben wurden. Dokumente können als E-Mail-Anlagen oder als OneDrive for Business-Links freigegeben werden, die in E-Mails gesendet werden.   |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.
```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
