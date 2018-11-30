---
title: Ressourcentyp resourceVisualization
description: Komplexer Typ mit Eigenschaften des Insights.
ms.openlocfilehash: 3ed61a8547e072938fc073d90f2592baf4c08fba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063205"
---
# <a name="resourcevisualization-resource-type"></a>Ressourcentyp resourceVisualization

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Komplexer Typ mit Eigenschaften des [Insights](insights.md).

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

```json
{
  "title": "string",
  "type"  : "string",
  "mediaType": "string",
  "previewImageUrl": "string",
  "previewText": "string",
  "containerWebUrl": "string",
  "containerDisplayName": "string",
  "containerType": "string"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft              | Typ          | Beschreibung  |
| -------------         |---------------| -------------|
| title                 | String        | Text für das Element.               |
| Typ              | String        | Medientyp für das Element. Kann zum Filtern von für eine bestimmte Datei auf Grundlage eines bestimmten Typs verwendet werden. Unterstützte Typen finden Sie weiter unten. |
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
-   Mail
-   CSV
-   Archiv
-   XPS
-   Audio
-   Video
-   Image
-   Web
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
-   Website
-   Mail
-   Ablage
-   Kasten
-   GDrive

Beispiel für eine Abfrage:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`