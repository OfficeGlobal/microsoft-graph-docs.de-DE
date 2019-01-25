---
title: Ressourcentyp visualInfo
description: Einen komplexen Typ für die **VisualElements** -Eigenschaft im Aktivitätsobjekt darstellt.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 56d3822c89de074847aeab6c8a0a742ecd7f006f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514922"
---
# <a name="visualinfo-resource-type"></a><span data-ttu-id="917d3-103">Ressourcentyp visualInfo</span><span class="sxs-lookup"><span data-stu-id="917d3-103">visualInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="917d3-104">Einen komplexen Typ für die **VisualElements** -Eigenschaft im [Aktivität](../resources/projectrome-activity.md) -Objekt darstellt.</span><span class="sxs-lookup"><span data-stu-id="917d3-104">A complex type for representing the **visualElements** property in the [activity](../resources/projectrome-activity.md) object.</span></span>

<span data-ttu-id="917d3-105">Jede Aktivität des Benutzers werden in Zeitachse wie eine Adaptive Karte angezeigt.</span><span class="sxs-lookup"><span data-stu-id="917d3-105">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="917d3-106">App-Entwickler werden empfohlen, eine benutzerdefinierte Karte angeben, die das Wesentliche der Aktivität erfasst wird, die in Ihrer app durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="917d3-106">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="917d3-107">Dies ist möglich, durch die Bereitstellung einer benutzerdefinierten JSON-Karte in die Content-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="917d3-107">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="917d3-108">Neben visual Metadaten mit einer Adaptive Karte app Content-Metadaten – Daten, die angeben, verwendet, um Rückschlüsse auf die Aktivität des Benutzers zu erstellen, um neue Aktivitäten für zukünftige erneute Engagements anbieten.</span><span class="sxs-lookup"><span data-stu-id="917d3-108">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="917d3-109">Dies ist möglich, mithilfe der Eigenschaft der Aktivität ContentInfo dar, ein JSON-Objekt anzugeben, der schema.org-Eigenschaften, um den Inhalt beschreiben nutzt.</span><span class="sxs-lookup"><span data-stu-id="917d3-109">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="917d3-110">Wenn eine benutzerdefinierte Karte nicht angegeben ist, wird eine einfache Karte mit Anzeigetext und Beschreibungseigenschaften generiert.</span><span class="sxs-lookup"><span data-stu-id="917d3-110">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="917d3-111">Benutzerdefinierte Karten werden empfohlen, um die besten Inhalte aus Ihrer App zu präsentieren.</span><span class="sxs-lookup"><span data-stu-id="917d3-111">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="917d3-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="917d3-112">Properties</span></span>

|<span data-ttu-id="917d3-113">Name</span><span class="sxs-lookup"><span data-stu-id="917d3-113">Name</span></span> | <span data-ttu-id="917d3-114">Typ</span><span class="sxs-lookup"><span data-stu-id="917d3-114">Type</span></span> | <span data-ttu-id="917d3-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="917d3-115">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="917d3-116">Anzeigetext</span><span class="sxs-lookup"><span data-stu-id="917d3-116">displayText</span></span> | <span data-ttu-id="917d3-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="917d3-117">String</span></span> | <span data-ttu-id="917d3-118">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="917d3-118">Required.</span></span> <span data-ttu-id="917d3-119">Kurze Beschreibung des Benutzers eindeutige Aktivität (beispielsweise Dokumentname in Fällen, in dem eine Aktivität zum Erstellen eines Dokuments bezieht sich)</span><span class="sxs-lookup"><span data-stu-id="917d3-119">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="917d3-120">description</span><span class="sxs-lookup"><span data-stu-id="917d3-120">description</span></span> | <span data-ttu-id="917d3-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="917d3-121">String</span></span> | <span data-ttu-id="917d3-122">Optional.</span><span class="sxs-lookup"><span data-stu-id="917d3-122">Optional.</span></span> <span data-ttu-id="917d3-123">Längere Beschreibung des eindeutigen Benutzeraktivität (Beispiel: Dokument-Namen, den ersten Satz und/oder Metadaten)</span><span class="sxs-lookup"><span data-stu-id="917d3-123">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="917d3-124">background-color</span><span class="sxs-lookup"><span data-stu-id="917d3-124">backgroundColor</span></span> | <span data-ttu-id="917d3-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="917d3-125">String</span></span> | <span data-ttu-id="917d3-126">Optional.</span><span class="sxs-lookup"><span data-stu-id="917d3-126">Optional.</span></span> <span data-ttu-id="917d3-127">Hintergrundfarbe verwendet, um die Aktivität in der UI - Marke Farbe für die Anwendungsquelle der Aktivität zu rendern.</span><span class="sxs-lookup"><span data-stu-id="917d3-127">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="917d3-128">Muss eine gültige hex Farbe</span><span class="sxs-lookup"><span data-stu-id="917d3-128">Must be a valid hex color</span></span>|
|<span data-ttu-id="917d3-129">content</span><span class="sxs-lookup"><span data-stu-id="917d3-129">content</span></span> | <span data-ttu-id="917d3-130">Nicht typisierte JSON-Objekt</span><span class="sxs-lookup"><span data-stu-id="917d3-130">Untyped JSON object</span></span> | <span data-ttu-id="917d3-131">Optional.</span><span class="sxs-lookup"><span data-stu-id="917d3-131">Optional.</span></span> <span data-ttu-id="917d3-132">Benutzerdefinierte Datenelement - JSON-Objekt verwendet, um benutzerdefinierte Inhalte für die Aktivität in der Windows-Shell UI Rendern bereitstellen</span><span class="sxs-lookup"><span data-stu-id="917d3-132">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="917d3-133">Zuweisung</span><span class="sxs-lookup"><span data-stu-id="917d3-133">attribution</span></span> | [<span data-ttu-id="917d3-134">imageInfo</span><span class="sxs-lookup"><span data-stu-id="917d3-134">imageInfo</span></span>](../resources/projectrome-imageinfo.md) | <span data-ttu-id="917d3-135">Optional.</span><span class="sxs-lookup"><span data-stu-id="917d3-135">Optional.</span></span> <span data-ttu-id="917d3-136">JSON-Objekt verwendet, um ein Symbol darstellen, die die Anwendung verwendet, um die Aktivität generieren darstellt</span><span class="sxs-lookup"><span data-stu-id="917d3-136">JSON object used to represent an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="917d3-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="917d3-137">JSON Representation</span></span>

<span data-ttu-id="917d3-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="917d3-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@data.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@data.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-visualinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
