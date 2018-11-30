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
# <a name="resourcevisualization-resource-type"></a><span data-ttu-id="4836d-103">Ressourcentyp resourceVisualization</span><span class="sxs-lookup"><span data-stu-id="4836d-103">resourceVisualization resource type</span></span>

> <span data-ttu-id="4836d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4836d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4836d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4836d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4836d-106">Komplexer Typ mit Eigenschaften des [Insights](insights.md).</span><span class="sxs-lookup"><span data-stu-id="4836d-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="4836d-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4836d-107">JSON representation</span></span>

<span data-ttu-id="4836d-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4836d-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="4836d-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4836d-109">Properties</span></span>

| <span data-ttu-id="4836d-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4836d-110">Property</span></span>              | <span data-ttu-id="4836d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="4836d-111">Type</span></span>          | <span data-ttu-id="4836d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4836d-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="4836d-113">title</span><span class="sxs-lookup"><span data-stu-id="4836d-113">title</span></span>                 | <span data-ttu-id="4836d-114">String</span><span class="sxs-lookup"><span data-stu-id="4836d-114">String</span></span>        | <span data-ttu-id="4836d-115">Text für das Element.</span><span class="sxs-lookup"><span data-stu-id="4836d-115">The item's title text.</span></span>               |
| <span data-ttu-id="4836d-116">Typ</span><span class="sxs-lookup"><span data-stu-id="4836d-116">type</span></span>              | <span data-ttu-id="4836d-117">String</span><span class="sxs-lookup"><span data-stu-id="4836d-117">String</span></span>        | <span data-ttu-id="4836d-118">Medientyp für das Element.</span><span class="sxs-lookup"><span data-stu-id="4836d-118">The item's media type.</span></span> <span data-ttu-id="4836d-119">Kann zum Filtern von für eine bestimmte Datei auf Grundlage eines bestimmten Typs verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="4836d-119">Can be used for filtering for a specific file based on a specific type.</span></span> <span data-ttu-id="4836d-120">Unterstützte Typen finden Sie weiter unten.</span><span class="sxs-lookup"><span data-stu-id="4836d-120">See below for supported types.</span></span> |
| <span data-ttu-id="4836d-121">mediaType</span><span class="sxs-lookup"><span data-stu-id="4836d-121">mediaType</span></span>             | <span data-ttu-id="4836d-122">String</span><span class="sxs-lookup"><span data-stu-id="4836d-122">String</span></span>        | <span data-ttu-id="4836d-123">Medientyp für das Element.</span><span class="sxs-lookup"><span data-stu-id="4836d-123">The item's media type.</span></span> <span data-ttu-id="4836d-124">Kann für verwendet werden, für die Filterung für einen bestimmten Typ der Datei basierend auf unterstützten IANA Media MIME-Typen.</span><span class="sxs-lookup"><span data-stu-id="4836d-124">Can be used for for filtering for a specific type of file based on supported IANA Media Mime Types.</span></span> <span data-ttu-id="4836d-125">Beachten Sie, dass nicht alle Medien MIME-Typen unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="4836d-125">Note that not all Media Mime Types are supported.</span></span> |
| <span data-ttu-id="4836d-126">Vorschaubild-URL</span><span class="sxs-lookup"><span data-stu-id="4836d-126">previewImageUrl</span></span>       | <span data-ttu-id="4836d-127">String</span><span class="sxs-lookup"><span data-stu-id="4836d-127">String</span></span>        | <span data-ttu-id="4836d-128">Eine URL für das Element des Vorschaubilds führende.</span><span class="sxs-lookup"><span data-stu-id="4836d-128">A URL leading to the preview image for the item.</span></span> |
| <span data-ttu-id="4836d-129">previewText</span><span class="sxs-lookup"><span data-stu-id="4836d-129">previewText</span></span>           | <span data-ttu-id="4836d-130">String</span><span class="sxs-lookup"><span data-stu-id="4836d-130">String</span></span>        | <span data-ttu-id="4836d-131">Eine Vorschautext für das Element.</span><span class="sxs-lookup"><span data-stu-id="4836d-131">A preview text for the item.</span></span> |
| <span data-ttu-id="4836d-132">containerWebUrl</span><span class="sxs-lookup"><span data-stu-id="4836d-132">containerWebUrl</span></span>       | <span data-ttu-id="4836d-133">String</span><span class="sxs-lookup"><span data-stu-id="4836d-133">String</span></span>        | <span data-ttu-id="4836d-134">Ein Pfad zu dem Ordner, in dem das Element gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="4836d-134">A path leading to the folder in which the item is stored.</span></span> |
| <span data-ttu-id="4836d-135">containerDisplayName</span><span class="sxs-lookup"><span data-stu-id="4836d-135">containerDisplayName</span></span>  | <span data-ttu-id="4836d-136">String</span><span class="sxs-lookup"><span data-stu-id="4836d-136">String</span></span>        | <span data-ttu-id="4836d-137">Eine Zeichenfolge, die beschreibt, in dem das Element gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="4836d-137">A string describing where the item is stored.</span></span> <span data-ttu-id="4836d-138">Beispielsweise der Name einer SharePoint-Website oder den Benutzernamen ein, die den Besitzer der OneDrive, speichern das Element identifiziert.</span><span class="sxs-lookup"><span data-stu-id="4836d-138">For example, the name of a SharePoint site or the user name identifying the owner of the OneDrive storing the item.</span></span>  |
| <span data-ttu-id="4836d-139">containerType</span><span class="sxs-lookup"><span data-stu-id="4836d-139">containerType</span></span>         | <span data-ttu-id="4836d-140">String</span><span class="sxs-lookup"><span data-stu-id="4836d-140">String</span></span> | <span data-ttu-id="4836d-141">Kann verwendet werden, zum Filtern nach der Typ des Containers, in dem die Datei gespeichert ist.</span><span class="sxs-lookup"><span data-stu-id="4836d-141">Can be used for filtering by the type of container in which the file is stored.</span></span> <span data-ttu-id="4836d-142">Wie Website oder OneDriveBusiness.</span><span class="sxs-lookup"><span data-stu-id="4836d-142">Such as Site or OneDriveBusiness.</span></span>       |

## <a name="type-property-values"></a><span data-ttu-id="4836d-143">Type-Eigenschaftenwerte</span><span class="sxs-lookup"><span data-stu-id="4836d-143">Type property values</span></span>
-   <span data-ttu-id="4836d-144">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="4836d-144">PowerPoint</span></span>
-   <span data-ttu-id="4836d-145">Word</span><span class="sxs-lookup"><span data-stu-id="4836d-145">Word</span></span>
-   <span data-ttu-id="4836d-146">Excel</span><span class="sxs-lookup"><span data-stu-id="4836d-146">Excel</span></span>
-   <span data-ttu-id="4836d-147">PDF-Datei</span><span class="sxs-lookup"><span data-stu-id="4836d-147">Pdf</span></span>
-   <span data-ttu-id="4836d-148">OneNote</span><span class="sxs-lookup"><span data-stu-id="4836d-148">OneNote</span></span>
-   <span data-ttu-id="4836d-149">OneNotePage</span><span class="sxs-lookup"><span data-stu-id="4836d-149">OneNotePage</span></span>
-   <span data-ttu-id="4836d-150">InfoPath</span><span class="sxs-lookup"><span data-stu-id="4836d-150">InfoPath</span></span>
-   <span data-ttu-id="4836d-151">Visio</span><span class="sxs-lookup"><span data-stu-id="4836d-151">Visio</span></span>
-   <span data-ttu-id="4836d-152">Publisher</span><span class="sxs-lookup"><span data-stu-id="4836d-152">Publisher</span></span>
-   <span data-ttu-id="4836d-153">Project</span><span class="sxs-lookup"><span data-stu-id="4836d-153">Project</span></span>
-   <span data-ttu-id="4836d-154">Access</span><span class="sxs-lookup"><span data-stu-id="4836d-154">Access</span></span>
-   <span data-ttu-id="4836d-155">Mail</span><span class="sxs-lookup"><span data-stu-id="4836d-155">Mail</span></span>
-   <span data-ttu-id="4836d-156">CSV</span><span class="sxs-lookup"><span data-stu-id="4836d-156">Csv</span></span>
-   <span data-ttu-id="4836d-157">Archiv</span><span class="sxs-lookup"><span data-stu-id="4836d-157">Archive</span></span>
-   <span data-ttu-id="4836d-158">XPS</span><span class="sxs-lookup"><span data-stu-id="4836d-158">Xps</span></span>
-   <span data-ttu-id="4836d-159">Audio</span><span class="sxs-lookup"><span data-stu-id="4836d-159">Audio</span></span>
-   <span data-ttu-id="4836d-160">Video</span><span class="sxs-lookup"><span data-stu-id="4836d-160">Video</span></span>
-   <span data-ttu-id="4836d-161">Image</span><span class="sxs-lookup"><span data-stu-id="4836d-161">Image</span></span>
-   <span data-ttu-id="4836d-162">Web</span><span class="sxs-lookup"><span data-stu-id="4836d-162">Web</span></span>
-   <span data-ttu-id="4836d-163">Text</span><span class="sxs-lookup"><span data-stu-id="4836d-163">Text</span></span>
-   <span data-ttu-id="4836d-164">XML</span><span class="sxs-lookup"><span data-stu-id="4836d-164">Xml</span></span>
-   <span data-ttu-id="4836d-165">Story</span><span class="sxs-lookup"><span data-stu-id="4836d-165">Story</span></span>
-   <span data-ttu-id="4836d-166">ExternalContent</span><span class="sxs-lookup"><span data-stu-id="4836d-166">ExternalContent</span></span>
-   <span data-ttu-id="4836d-167">Ordner</span><span class="sxs-lookup"><span data-stu-id="4836d-167">Folder</span></span>
-   <span data-ttu-id="4836d-168">Andere</span><span class="sxs-lookup"><span data-stu-id="4836d-168">Other</span></span>

<span data-ttu-id="4836d-169">Beispiel für eine Abfrage:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span><span class="sxs-lookup"><span data-stu-id="4836d-169">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`</span></span>

## <a name="containertype-property-values"></a><span data-ttu-id="4836d-170">ContainerType-Eigenschaftswerte</span><span class="sxs-lookup"><span data-stu-id="4836d-170">containerType property values</span></span>
<span data-ttu-id="4836d-171">Unterstützten Typen können basierend auf Container unterscheiden sich aus denen die [Erkenntnisse](insights.md) Dateien zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4836d-171">The supported types can differ based on containers from which the [Insight](insights.md) returns files.</span></span> <span data-ttu-id="4836d-172">Beispielsweise gibt nur die [Shared](insights-shared.md) Einblicke Dateien aus 'Ablage', 'Feld' und 'GDrive' zurück.</span><span class="sxs-lookup"><span data-stu-id="4836d-172">For example, only the [Shared](insights-shared.md) insight returns files from 'DropBox', 'Box', and 'GDrive'.</span></span>

-   <span data-ttu-id="4836d-173">OneDriveBusiness</span><span class="sxs-lookup"><span data-stu-id="4836d-173">OneDriveBusiness</span></span>
-   <span data-ttu-id="4836d-174">Website</span><span class="sxs-lookup"><span data-stu-id="4836d-174">Site</span></span>
-   <span data-ttu-id="4836d-175">Mail</span><span class="sxs-lookup"><span data-stu-id="4836d-175">Mail</span></span>
-   <span data-ttu-id="4836d-176">Ablage</span><span class="sxs-lookup"><span data-stu-id="4836d-176">DropBox</span></span>
-   <span data-ttu-id="4836d-177">Kasten</span><span class="sxs-lookup"><span data-stu-id="4836d-177">Box</span></span>
-   <span data-ttu-id="4836d-178">GDrive</span><span class="sxs-lookup"><span data-stu-id="4836d-178">GDrive</span></span>

<span data-ttu-id="4836d-179">Beispiel für eine Abfrage:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span><span class="sxs-lookup"><span data-stu-id="4836d-179">Example query: `https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`</span></span>