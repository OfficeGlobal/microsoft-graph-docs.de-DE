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
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="82c3b-103">Ressourcentyp resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="82c3b-103">resourceVisualization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82c3b-104">Komplexer Typ mit Eigenschaften des [OfficeGraphInsights](insights.md).</span><span class="sxs-lookup"><span data-stu-id="82c3b-104">Complex type containing properties of [officeGraphInsights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="82c3b-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="82c3b-105">JSON representation</span></span>

<span data-ttu-id="82c3b-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="82c3b-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="82c3b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="82c3b-107">Properties</span></span>

| <span data-ttu-id="82c3b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="82c3b-108">Property</span></span>              | <span data-ttu-id="82c3b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="82c3b-109">Type</span></span>          | <span data-ttu-id="82c3b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82c3b-110">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="82c3b-111">title</span><span class="sxs-lookup"><span data-stu-id="82c3b-111">title</span></span>                 | <span data-ttu-id="82c3b-112">String</span><span class="sxs-lookup"><span data-stu-id="82c3b-112">String</span></span>        | <span data-ttu-id="82c3b-113">Text für das Element.</span><span class="sxs-lookup"><span data-stu-id="82c3b-113">The item's title text.</span></span>               |
| <span data-ttu-id="82c3b-114">type</span><span class="sxs-lookup"><span data-stu-id="82c3b-114">type</span></span>              | <span data-ttu-id="82c3b-115">String</span><span class="sxs-lookup"><span data-stu-id="82c3b-115">String</span></span>        | <span data-ttu-id="82c3b-116">Medientyp für das Element.</span><span class="sxs-lookup"><span data-stu-id="82c3b-116">The item's media type.</span></span> <span data-ttu-id="82c3b-117">Kann zum Filtern von für eine bestimmte Datei auf Grundlage eines bestimmten Typs verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="82c3b-117">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="82c3b-118">Unterstützte Typen finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="82c3b-118">See below for supported types.</span></span> |
| <span data-ttu-id="82c3b-119">mediaType</span><span class="sxs-lookup"><span data-stu-id="82c3b-119">mediaType</span></span>             | <span data-ttu-id="82c3b-120">String</span><span class="sxs-lookup"><span data-stu-id="82c3b-120">String</span></span>        | <span data-ttu-id="82c3b-121">Medientyp für das Element.</span><span class="sxs-lookup"><span data-stu-id="82c3b-121">The item's media type.</span></span> <span data-ttu-id="82c3b-122">Kann für verwendet werden, für die Filterung für einen bestimmten Typ der Datei basierend auf unterstützten IANA Media MIME-Typen.</span><span class="sxs-lookup"><span data-stu-id="82c3b-122">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="82c3b-123">Beachten Sie, dass nicht alle Medien MIME-Typen unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="82c3b-123">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="82c3b-124">Vorschaubild-URL</span><span class="sxs-lookup"><span data-stu-id="82c3b-124">previewImageUrl</span></span>       | <span data-ttu-id="82c3b-125">String</span><span class="sxs-lookup"><span data-stu-id="82c3b-125">String</span></span>        | <span data-ttu-id="82c3b-126">Eine URL für das Element des Vorschaubilds führende.</span><span class="sxs-lookup"><span data-stu-id="82c3b-126">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="82c3b-127">previewText</span><span class="sxs-lookup"><span data-stu-id="82c3b-127">previewText</span></span>           | <span data-ttu-id="82c3b-128">String</span><span class="sxs-lookup"><span data-stu-id="82c3b-128">String</span></span>        | <span data-ttu-id="82c3b-129">Eine Vorschautext für das Element.</span><span class="sxs-lookup"><span data-stu-id="82c3b-129">A preview text for the item.</span></span> |
| <span data-ttu-id="82c3b-130">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="82c3b-130">containerWebUrl</span></span>       | <span data-ttu-id="82c3b-131">String</span><span class="sxs-lookup"><span data-stu-id="82c3b-131">String</span></span>        | <span data-ttu-id="82c3b-132">Ein Pfad zu dem Ordner, in dem das Element gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="82c3b-132">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="82c3b-133">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="82c3b-133">containerDisplayName</span></span>  | <span data-ttu-id="82c3b-134">String</span><span class="sxs-lookup"><span data-stu-id="82c3b-134">String</span></span>        | <span data-ttu-id="82c3b-135">Eine Zeichenfolge, die beschreibt, in dem das Element gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="82c3b-135">A string describing where the item is stored.</span></span> <span data-ttu-id="82c3b-136">Beispielsweise der Name einer SharePoint-Website oder den Benutzernamen ein, die den Besitzer der OneDrive, speichern das Element identifiziert.</span><span class="sxs-lookup"><span data-stu-id="82c3b-136">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="82c3b-137">containerType</span><span class="sxs-lookup"><span data-stu-id="82c3b-137">containerType</span></span>         | <span data-ttu-id="82c3b-138">String</span><span class="sxs-lookup"><span data-stu-id="82c3b-138">String</span></span> | <span data-ttu-id="82c3b-139">Kann verwendet werden, zum Filtern nach der Typ des Containers, in dem die Datei gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="82c3b-139">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="82c3b-140">Wie Website oder OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="82c3b-140">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="82c3b-141">Type-Eigenschaftenwerte</span><span class="sxs-lookup"><span data-stu-id="82c3b-141">Type property values</span></span>
-   <span data-ttu-id="82c3b-142">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="82c3b-142">PowerPoint</span></span>
-   <span data-ttu-id="82c3b-143">Word</span><span class="sxs-lookup"><span data-stu-id="82c3b-143">Word</span></span>
-   <span data-ttu-id="82c3b-144">Excel</span><span class="sxs-lookup"><span data-stu-id="82c3b-144">Excel</span></span>
-   <span data-ttu-id="82c3b-145">PDF-Datei</span><span class="sxs-lookup"><span data-stu-id="82c3b-145">Pdf</span></span>
-   <span data-ttu-id="82c3b-146">OneNote</span><span class="sxs-lookup"><span data-stu-id="82c3b-146">OneNote</span></span>
-   <span data-ttu-id="82c3b-147">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="82c3b-147">OneNotePage</span></span>
-   <span data-ttu-id="82c3b-148">InfoPath</span><span class="sxs-lookup"><span data-stu-id="82c3b-148">InfoPath</span></span>
-   <span data-ttu-id="82c3b-149">Visio</span><span class="sxs-lookup"><span data-stu-id="82c3b-149">Visio</span></span>
-   <span data-ttu-id="82c3b-150">Publisher</span><span class="sxs-lookup"><span data-stu-id="82c3b-150">Publisher</span></span>
-   <span data-ttu-id="82c3b-151">Project</span><span class="sxs-lookup"><span data-stu-id="82c3b-151">Project</span></span>
-   <span data-ttu-id="82c3b-152">Access</span><span class="sxs-lookup"><span data-stu-id="82c3b-152">Access</span></span>
-   <span data-ttu-id="82c3b-153">E-Mail</span><span class="sxs-lookup"><span data-stu-id="82c3b-153">Mail</span></span>
-   <span data-ttu-id="82c3b-154">CSV</span><span class="sxs-lookup"><span data-stu-id="82c3b-154">Csv</span></span>
-   <span data-ttu-id="82c3b-155">Archiv</span><span class="sxs-lookup"><span data-stu-id="82c3b-155">Archive</span></span>
-   <span data-ttu-id="82c3b-156">XPS</span><span class="sxs-lookup"><span data-stu-id="82c3b-156">Xps</span></span>
-   <span data-ttu-id="82c3b-157">Audio</span><span class="sxs-lookup"><span data-stu-id="82c3b-157">Audio</span></span>
-   <span data-ttu-id="82c3b-158">Video</span><span class="sxs-lookup"><span data-stu-id="82c3b-158">Video</span></span>
-   <span data-ttu-id="82c3b-159">Bild</span><span class="sxs-lookup"><span data-stu-id="82c3b-159">Image</span></span>
-   <span data-ttu-id="82c3b-160">Netz</span><span class="sxs-lookup"><span data-stu-id="82c3b-160">Web</span></span>
-   <span data-ttu-id="82c3b-161">Text</span><span class="sxs-lookup"><span data-stu-id="82c3b-161">Text</span></span>
-   <span data-ttu-id="82c3b-162">XML</span><span class="sxs-lookup"><span data-stu-id="82c3b-162">Xml</span></span>
-   <span data-ttu-id="82c3b-163">Story</span><span class="sxs-lookup"><span data-stu-id="82c3b-163">Story</span></span>
-   <span data-ttu-id="82c3b-164">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="82c3b-164">ExternalContent</span></span>
-   <span data-ttu-id="82c3b-165">Ordner</span><span class="sxs-lookup"><span data-stu-id="82c3b-165">Folder</span></span>
-   <span data-ttu-id="82c3b-166">Andere</span><span class="sxs-lookup"><span data-stu-id="82c3b-166">Other</span></span>

<span data-ttu-id="82c3b-167">Beispiel für eine Abfrage:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="82c3b-167">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="82c3b-168">ContainerType-Eigenschaftswerte</span><span class="sxs-lookup"><span data-stu-id="82c3b-168">containerType property values</span></span>
<span data-ttu-id="82c3b-169">Unterstützten Typen können basierend auf Container unterscheiden sich aus denen die [Erkenntnisse](insights.md) Dateien zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="82c3b-169">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="82c3b-170">Beispielsweise gibt nur die [Shared](insights-shared.md) Einblicke Dateien aus 'Ablage', 'Feld' und 'GDrive' zurück.</span><span class="sxs-lookup"><span data-stu-id="82c3b-170">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="82c3b-171">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="82c3b-171">OneDriveBusiness</span></span>
-   <span data-ttu-id="82c3b-172">Site</span><span class="sxs-lookup"><span data-stu-id="82c3b-172">Site</span></span>
-   <span data-ttu-id="82c3b-173">E-Mail</span><span class="sxs-lookup"><span data-stu-id="82c3b-173">Mail</span></span>
-   <span data-ttu-id="82c3b-174">Ablage</span><span class="sxs-lookup"><span data-stu-id="82c3b-174">DropBox</span></span>
-   <span data-ttu-id="82c3b-175">Kasten</span><span class="sxs-lookup"><span data-stu-id="82c3b-175">Box</span></span>
-   <span data-ttu-id="82c3b-176">GDrive</span><span class="sxs-lookup"><span data-stu-id="82c3b-176">GDrive</span></span>

<span data-ttu-id="82c3b-177">Beispiel für eine Abfrage:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="82c3b-177">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
