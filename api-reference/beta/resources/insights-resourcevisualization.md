---
title: Ressourcentyp resourceVisualization
description: Komplexer Typ mit Eigenschaften des Insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 9dc2d50a5bc694204317f8c3332263ce5259e2fc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575104"
---
# <a name="resourcevisualization-resource-type"></a>Ressourcentyp resourceVisualization

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Komplexer Typ mit Eigenschaften des [OfficeGraphInsights](insights.md).

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],  
  "@odata.type": "microsoft.graph.resourceVisualization"
}-->
```json
{
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft              | Typ          | Beschreibung  |
| -------------         |---------------| -------------|
| title                 | String        | Text für das Element.               |
| type              | String        | Medientyp für das Element. Kann zum Filtern von für eine bestimmte Datei auf Grundlage eines bestimmten Typs verwendet werden. Unterstützte Typen finden Sie weiter unten. |
| mediaType             | String        | Medientyp für das Element. Kann für verwendet werden, für die Filterung für einen bestimmten Typ der Datei basierend auf unterstützten IANA Media MIME-Typen. Beachten Sie, dass nicht alle Medien MIME-Typen unterstützt werden. |
| Vorschaubild-URL       | String        | Eine URL für das Element des Vorschaubilds führende. |
| previewText           | String        | Eine Vorschautext für das Element. |
| containerWebUrl       | String        | Ein Pfad zu dem Ordner, in dem das Element gespeichert ist. |
| containerDisplayName  | String        | Eine Zeichenfolge, die beschreibt, in dem das Element gespeichert ist. Beispielsweise der Name einer SharePoint-Website oder den Benutzernamen ein, die den Besitzer der OneDrive, speichern das Element identifiziert.  |
| containerType         | String | Kann verwendet werden, zum Filtern nach der Typ des Containers, in dem die Datei gespeichert ist. Wie Website oder OneDriveBusiness.       |

## <a name="type-property-values"></a>Type-Eigenschaftenwerte
-   PowerPoint
-   Word
-   Excel
-   PDF-Datei
-   OneNote
-   OneNotePage
-   InfoPath
-   Visio
-   Publisher
-   Project
-   Access
-   E-Mail
-   CSV
-   Archiv
-   XPS
-   Audio
-   Video
-   Bild
-   Netz
-   Text
-   XML
-   Story
-   ExternalContent
-   Ordner
-   Andere

Beispiel für eine Abfrage:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

## <a name="containertype-property-values"></a>ContainerType-Eigenschaftswerte
Unterstützten Typen können basierend auf Container unterscheiden sich aus denen die [Erkenntnisse](insights.md) Dateien zurückgegeben. Beispielsweise gibt nur die [Shared](insights-shared.md) Einblicke Dateien aus 'Ablage', 'Feld' und 'GDrive' zurück.

-   OneDriveBusiness
-   Site
-   E-Mail
-   Ablage
-   Kasten
-   GDrive

Beispiel für eine Abfrage:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
