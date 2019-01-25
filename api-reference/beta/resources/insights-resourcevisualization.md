---
title: Ressourcentyp resourceVisualization
description: Komplexer Typ mit Eigenschaften des Insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ec1619d07d0f31bf8325c25b161084f505b3ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526760"
---
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="440dd-103">Ressourcentyp resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="440dd-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="440dd-104">Komplexer Typ mit Eigenschaften des [Insights](insights.md).</span><span class="sxs-lookup"><span data-stu-id="440dd-104">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="440dd-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="440dd-105">JSON representation</span></span>

<span data-ttu-id="440dd-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="440dd-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="440dd-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="440dd-107">Properties</span></span>

| <span data-ttu-id="440dd-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="440dd-108">Property</span></span>              | <span data-ttu-id="440dd-109">Typ</span><span class="sxs-lookup"><span data-stu-id="440dd-109">Type</span></span>          | <span data-ttu-id="440dd-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="440dd-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="440dd-111">title</span><span class="sxs-lookup"><span data-stu-id="440dd-111">title</span></span>                 | <span data-ttu-id="440dd-112">String</span><span class="sxs-lookup"><span data-stu-id="440dd-112">String</span></span>        | <span data-ttu-id="440dd-113">Text für das Element.</span><span class="sxs-lookup"><span data-stu-id="440dd-113">The item's title text.</span></span>               |
| <span data-ttu-id="440dd-114">type</span><span class="sxs-lookup"><span data-stu-id="440dd-114">type</span></span>              | <span data-ttu-id="440dd-115">String</span><span class="sxs-lookup"><span data-stu-id="440dd-115">String</span></span>        | <span data-ttu-id="440dd-116">Medientyp für das Element.</span><span class="sxs-lookup"><span data-stu-id="440dd-116">The item's media type.</span></span> <span data-ttu-id="440dd-117">Kann zum Filtern von für eine bestimmte Datei auf Grundlage eines bestimmten Typs verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="440dd-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="440dd-118">Unterstützte Typen finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="440dd-118">See below for supported types.</span></span> |
| <span data-ttu-id="440dd-119">MediaType</span><span class="sxs-lookup"><span data-stu-id="440dd-119">mediaType</span></span>             | <span data-ttu-id="440dd-120">String</span><span class="sxs-lookup"><span data-stu-id="440dd-120">String</span></span>        | <span data-ttu-id="440dd-121">Medientyp für das Element.</span><span class="sxs-lookup"><span data-stu-id="440dd-121">The item's media type.</span></span> <span data-ttu-id="440dd-122">Kann für verwendet werden, für die Filterung für einen bestimmten Typ der Datei basierend auf unterstützten IANA Media MIME-Typen.</span><span class="sxs-lookup"><span data-stu-id="440dd-122">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="440dd-123">Beachten Sie, dass nicht alle Medien MIME-Typen unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="440dd-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="440dd-124">PreviewImageUrl</span><span class="sxs-lookup"><span data-stu-id="440dd-124">previewImageUrl</span></span>       | <span data-ttu-id="440dd-125">String</span><span class="sxs-lookup"><span data-stu-id="440dd-125">String</span></span>        | <span data-ttu-id="440dd-126">Eine URL für das Element des Vorschaubilds führende.</span><span class="sxs-lookup"><span data-stu-id="440dd-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="440dd-127">previewText</span><span class="sxs-lookup"><span data-stu-id="440dd-127">previewText</span></span>           | <span data-ttu-id="440dd-128">String</span><span class="sxs-lookup"><span data-stu-id="440dd-128">String</span></span>        | <span data-ttu-id="440dd-129">Eine Vorschautext für das Element.</span><span class="sxs-lookup"><span data-stu-id="440dd-129">A preview text for the item.</span></span> |
| <span data-ttu-id="440dd-130">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="440dd-130">containerWebUrl</span></span>       | <span data-ttu-id="440dd-131">String</span><span class="sxs-lookup"><span data-stu-id="440dd-131">String</span></span>        | <span data-ttu-id="440dd-132">Ein Pfad zu dem Ordner, in dem das Element gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="440dd-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="440dd-133">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="440dd-133">containerDisplayName</span></span>  | <span data-ttu-id="440dd-134">String</span><span class="sxs-lookup"><span data-stu-id="440dd-134">String</span></span>        | <span data-ttu-id="440dd-135">Eine Zeichenfolge, die beschreibt, in dem das Element gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="440dd-135">A string describing where the item is stored.</span></span> <span data-ttu-id="440dd-136">Beispielsweise der Name einer SharePoint-Website oder den Benutzernamen ein, die den Besitzer der OneDrive, speichern das Element identifiziert.</span><span class="sxs-lookup"><span data-stu-id="440dd-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="440dd-137">ContainerType</span><span class="sxs-lookup"><span data-stu-id="440dd-137">containerType</span></span>         | <span data-ttu-id="440dd-138">String</span><span class="sxs-lookup"><span data-stu-id="440dd-138">String</span></span> | <span data-ttu-id="440dd-139">Kann verwendet werden, zum Filtern nach der Typ des Containers, in dem die Datei gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="440dd-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="440dd-140">Wie Website oder OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="440dd-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="440dd-141">Type-Eigenschaftenwerte</span><span class="sxs-lookup"><span data-stu-id="440dd-141">Type property values</span></span>
-   <span data-ttu-id="440dd-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="440dd-142">PowerPoint</span></span>
-   <span data-ttu-id="440dd-143">Word</span><span class="sxs-lookup"><span data-stu-id="440dd-143">Word</span></span>
-   <span data-ttu-id="440dd-144">Excel</span><span class="sxs-lookup"><span data-stu-id="440dd-144">Excel</span></span>
-   <span data-ttu-id="440dd-145">PDF</span><span class="sxs-lookup"><span data-stu-id="440dd-145">Pdf</span></span>
-   <span data-ttu-id="440dd-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="440dd-146">OneNote</span></span>
-   <span data-ttu-id="440dd-147">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="440dd-147">OneNotePage</span></span>
-   <span data-ttu-id="440dd-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="440dd-148">InfoPath</span></span>
-   <span data-ttu-id="440dd-149">Visio</span><span class="sxs-lookup"><span data-stu-id="440dd-149">Visio</span></span>
-   <span data-ttu-id="440dd-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="440dd-150">Publisher</span></span>
-   <span data-ttu-id="440dd-151">Project</span><span class="sxs-lookup"><span data-stu-id="440dd-151">Project</span></span>
-   <span data-ttu-id="440dd-152">Access</span><span class="sxs-lookup"><span data-stu-id="440dd-152">Access</span></span>
-   <span data-ttu-id="440dd-153">E-Mail</span><span class="sxs-lookup"><span data-stu-id="440dd-153">Mail</span></span>
-   <span data-ttu-id="440dd-154">CSV</span><span class="sxs-lookup"><span data-stu-id="440dd-154">Csv</span></span>
-   <span data-ttu-id="440dd-155">Archiv</span><span class="sxs-lookup"><span data-stu-id="440dd-155">Archive</span></span>
-   <span data-ttu-id="440dd-156">XPS</span><span class="sxs-lookup"><span data-stu-id="440dd-156">Xps</span></span>
-   <span data-ttu-id="440dd-157">Audio</span><span class="sxs-lookup"><span data-stu-id="440dd-157">Audio</span></span>
-   <span data-ttu-id="440dd-158">Video</span><span class="sxs-lookup"><span data-stu-id="440dd-158">Video</span></span>
-   <span data-ttu-id="440dd-159">Bild</span><span class="sxs-lookup"><span data-stu-id="440dd-159">Image</span></span>
-   <span data-ttu-id="440dd-160">Netz</span><span class="sxs-lookup"><span data-stu-id="440dd-160">Web</span></span>
-   <span data-ttu-id="440dd-161">Text</span><span class="sxs-lookup"><span data-stu-id="440dd-161">Text</span></span>
-   <span data-ttu-id="440dd-162">XML</span><span class="sxs-lookup"><span data-stu-id="440dd-162">Xml</span></span>
-   <span data-ttu-id="440dd-163">Story</span><span class="sxs-lookup"><span data-stu-id="440dd-163">Story</span></span>
-   <span data-ttu-id="440dd-164">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="440dd-164">ExternalContent</span></span>
-   <span data-ttu-id="440dd-165">Ordner</span><span class="sxs-lookup"><span data-stu-id="440dd-165">Folder</span></span>
-   <span data-ttu-id="440dd-166">Andere</span><span class="sxs-lookup"><span data-stu-id="440dd-166">Other</span></span>

<span data-ttu-id="440dd-167">Beispiel für eine Abfrage:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="440dd-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="440dd-168">ContainerType-Eigenschaftswerte</span><span class="sxs-lookup"><span data-stu-id="440dd-168">containerType property values</span></span>
<span data-ttu-id="440dd-169">Unterstützten Typen können basierend auf Container unterscheiden sich aus denen die [Erkenntnisse](insights.md) Dateien zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="440dd-169">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="440dd-170">Beispielsweise gibt nur die [Shared](insights-shared.md) Einblicke Dateien aus 'Ablage', 'Feld' und 'GDrive' zurück.</span><span class="sxs-lookup"><span data-stu-id="440dd-170">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="440dd-171">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="440dd-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="440dd-172">Site</span><span class="sxs-lookup"><span data-stu-id="440dd-172">Site</span></span>
-   <span data-ttu-id="440dd-173">E-Mail</span><span class="sxs-lookup"><span data-stu-id="440dd-173">Mail</span></span>
-   <span data-ttu-id="440dd-174">Ablage</span><span class="sxs-lookup"><span data-stu-id="440dd-174">DropBox</span></span>
-   <span data-ttu-id="440dd-175">Kasten</span><span class="sxs-lookup"><span data-stu-id="440dd-175">Box</span></span>
-   <span data-ttu-id="440dd-176">GDrive</span><span class="sxs-lookup"><span data-stu-id="440dd-176">GDrive</span></span>

<span data-ttu-id="440dd-177">Beispiel für eine Abfrage:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="440dd-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
