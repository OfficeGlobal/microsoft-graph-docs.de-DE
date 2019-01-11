---
title: Ressourcentyp visualInfo
description: Einen komplexen Typ für die **VisualElements** -Eigenschaft im Aktivitätsobjekt darstellt.
localization_priority: Normal
ms.openlocfilehash: 3e1dd3d7e4ecfaf5053f839f0ac0d0039692b2a4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855314"
---
# <a name="visualinfo-resource-type"></a><span data-ttu-id="dbbcf-103">Ressourcentyp visualInfo</span><span class="sxs-lookup"><span data-stu-id="dbbcf-103">visualInfo resource type</span></span>

> <span data-ttu-id="dbbcf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbbcf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbbcf-106">Einen komplexen Typ für die **VisualElements** -Eigenschaft im [Aktivität](../resources/projectrome-activity.md) -Objekt darstellt.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-106">A complex type for representing the **visualElements** property in the [activity](../resources/projectrome-activity.md) object.</span></span>

<span data-ttu-id="dbbcf-107">Jede Aktivität des Benutzers werden in Zeitachse wie eine Adaptive Karte angezeigt.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-107">Each user activity will be shown in Timeline as an Adaptive Card.</span></span> <span data-ttu-id="dbbcf-108">App-Entwickler werden empfohlen, eine benutzerdefinierte Karte angeben, die das Wesentliche der Aktivität erfasst wird, die in Ihrer app durchgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-108">App developers are encouraged to provide a custom Card which captures the essence of the activity which took place in your app.</span></span> <span data-ttu-id="dbbcf-109">Dies ist möglich, durch die Bereitstellung einer benutzerdefinierten JSON-Karte in die Content-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-109">This is possible by providing a custom JSON card in the content property.</span></span>

<span data-ttu-id="dbbcf-110">Neben visual Metadaten mit einer Adaptive Karte app Content-Metadaten – Daten, die angeben, verwendet, um Rückschlüsse auf die Aktivität des Benutzers zu erstellen, um neue Aktivitäten für zukünftige erneute Engagements anbieten.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-110">In addition to visual metadata with an Adaptive Card, app can specify content metadata – data that be used to build inferences on the user’s activity in order to offer new activities for future re-engagement.</span></span> <span data-ttu-id="dbbcf-111">Dies ist möglich, mithilfe der Eigenschaft der Aktivität ContentInfo dar, ein JSON-Objekt anzugeben, der schema.org-Eigenschaften, um den Inhalt beschreiben nutzt.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-111">This is possible by using the activity's contentInfo property to provide a JSON object which leverages schema.org properties to describe the content.</span></span>

<span data-ttu-id="dbbcf-112">Wenn eine benutzerdefinierte Karte nicht angegeben ist, wird eine einfache Karte mit Anzeigetext und Beschreibungseigenschaften generiert.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-112">If a custom card is not provided, a simple card will be generated using displayText and description properties.</span></span> <span data-ttu-id="dbbcf-113">Benutzerdefinierte Karten werden empfohlen, um die besten Inhalte aus Ihrer App zu präsentieren.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-113">Custom cards are recommended to showcase the best content from within your app.</span></span>

## <a name="properties"></a><span data-ttu-id="dbbcf-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dbbcf-114">Properties</span></span>

|<span data-ttu-id="dbbcf-115">Name</span><span class="sxs-lookup"><span data-stu-id="dbbcf-115">Name</span></span> | <span data-ttu-id="dbbcf-116">Typ</span><span class="sxs-lookup"><span data-stu-id="dbbcf-116">Type</span></span> | <span data-ttu-id="dbbcf-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dbbcf-117">Description</span></span>|
|:----|:------|:-----------|
|<span data-ttu-id="dbbcf-118">Anzeigetext</span><span class="sxs-lookup"><span data-stu-id="dbbcf-118">displayText</span></span> | <span data-ttu-id="dbbcf-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dbbcf-119">String</span></span> | <span data-ttu-id="dbbcf-120">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-120">Required.</span></span> <span data-ttu-id="dbbcf-121">Kurze Beschreibung des Benutzers eindeutige Aktivität (beispielsweise Dokumentname in Fällen, in dem eine Aktivität zum Erstellen eines Dokuments bezieht sich)</span><span class="sxs-lookup"><span data-stu-id="dbbcf-121">Short text description of the user's unique activity (for example, document name in cases where an activity refers to document creation)</span></span>|
|<span data-ttu-id="dbbcf-122">description</span><span class="sxs-lookup"><span data-stu-id="dbbcf-122">description</span></span> | <span data-ttu-id="dbbcf-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dbbcf-123">String</span></span> | <span data-ttu-id="dbbcf-124">Optional.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-124">Optional.</span></span> <span data-ttu-id="dbbcf-125">Längere Beschreibung des eindeutigen Benutzeraktivität (Beispiel: Dokument-Namen, den ersten Satz und/oder Metadaten)</span><span class="sxs-lookup"><span data-stu-id="dbbcf-125">Longer text description of the user's unique activity (example: document name, first sentence, and/or metadata)</span></span>|
|<span data-ttu-id="dbbcf-126">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="dbbcf-126">backgroundColor</span></span> | <span data-ttu-id="dbbcf-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dbbcf-127">String</span></span> | <span data-ttu-id="dbbcf-128">Optional.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-128">Optional.</span></span> <span data-ttu-id="dbbcf-129">Hintergrundfarbe verwendet, um die Aktivität in der UI - Marke Farbe für die Anwendungsquelle der Aktivität zu rendern.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-129">Background color used to render the activity in the UI - brand color for the application source of the activity.</span></span> <span data-ttu-id="dbbcf-130">Muss eine gültige hex Farbe</span><span class="sxs-lookup"><span data-stu-id="dbbcf-130">Must be a valid hex color</span></span>|
|<span data-ttu-id="dbbcf-131">content</span><span class="sxs-lookup"><span data-stu-id="dbbcf-131">content</span></span> | <span data-ttu-id="dbbcf-132">Nicht typisierte JSON-Objekt</span><span class="sxs-lookup"><span data-stu-id="dbbcf-132">Untyped JSON object</span></span> | <span data-ttu-id="dbbcf-133">Optional.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-133">Optional.</span></span> <span data-ttu-id="dbbcf-134">Benutzerdefinierte Datenelement - JSON-Objekt verwendet, um benutzerdefinierte Inhalte für die Aktivität in der Windows-Shell UI Rendern bereitstellen</span><span class="sxs-lookup"><span data-stu-id="dbbcf-134">Custom piece of data - JSON object used to provide custom content to render the activity in the Windows Shell UI</span></span>|
|<span data-ttu-id="dbbcf-135">Zuweisung</span><span class="sxs-lookup"><span data-stu-id="dbbcf-135">attribution</span></span> | [<span data-ttu-id="dbbcf-136">imageInfo</span><span class="sxs-lookup"><span data-stu-id="dbbcf-136">imageInfo</span></span>](../resources/projectrome-imageinfo.md) | <span data-ttu-id="dbbcf-137">Optional.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-137">Optional.</span></span> <span data-ttu-id="dbbcf-138">JSON-Objekt verwendet, um ein Symbol darstellen, die die Anwendung verwendet, um die Aktivität generieren darstellt</span><span class="sxs-lookup"><span data-stu-id="dbbcf-138">JSON object used to represent an icon which represents the application used to generate the activity</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dbbcf-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dbbcf-139">JSON Representation</span></span>

<span data-ttu-id="dbbcf-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dbbcf-140">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
